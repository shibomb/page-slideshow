<template>
  <v-sheet class="w-100 h-100">
    <transition v-show="fade">
      <v-sheet class="w-100 h-100">
        <v-img
          v-if="content.type == 'asset-image'"
          :src="convertImgSrc(content.url)"
        />
        <v-img v-if="content.type == 'image'" :src="content.url" />
        <iframe
          v-if="content.type == 'iframe'"
          :src="content.url"
          width="100%"
          height="100%"
        />
      </v-sheet>
    </transition>
  </v-sheet>
</template>

<style>
.v-enter-active,
.v-leave-active {
  transition: opacity v-bind(transitionTimeStr) ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}
</style>

<script lang="ts">
// <v-sheet class="w-100">
//   <v-card-actions>
//     <v-btn class="btn btn-default" @click="current--">&lt;</v-btn>
//     <v-spacer></v-spacer>
//     <v-btn class="btn btn-default" @click="current--">||</v-btn>
//     <v-spacer></v-spacer>
//     <v-btn class="btn btn-default" @click="current++">&gt;</v-btn>
//   </v-card-actions>
// </v-sheet>

interface ContentInfo {
  type: string;
  url: string;
}
</script>

<script lang="ts" setup>
import { PropType, computed, onMounted, ref } from "vue";

const props = defineProps({
  contents: {
    type: Array as PropType<ContentInfo[]>,
    default: () => [],
    require: true,
  },
  interval: {
    type: Number,
    default: 6000,
    require: false,
  },
  transitionTime: {
    type: Number,
    default: 1000,
    require: false,
  },
});

const timer = ref({});
const fade = ref(true);
const current: any = ref(0);

const content = computed(() => {
  return props.contents[current.value];
});

const transitionTimeStr = computed(() => {
  return props.transitionTime + "ms";
});

onMounted(() => {
  console.log("#mounted");
  timer.value = setInterval(next, props.interval);
});

const next = () => {
  fade.value = false;
  setTimeout(() => {
    current.value = (current.value + 1) % props.contents.length;
  }, props.transitionTime);

  setTimeout(() => {
    fade.value = true;
  }, props.transitionTime * 2);
};

const convertImgSrc = (url: string): string => {
  return new URL(url, import.meta.url).href;
};
</script>
