<template>
  <page-slideshow
    :contents="contents"
    :interval="30000"
    :transition-time="1000"
  ></page-slideshow>
</template>

<script lang="ts" setup>
import PageSlideshow from "@/components/PageSlideshow.vue";

const contents = [
  // {
  //   type: "iframe",
  //   url: "https://shibomb.xyz",
  // },
  // {
  //   type: "iframe",
  //   url: "https://editor.p5js.org/shibomb/full/VrjLFyhSq",
  // },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/k0q_SyCyy",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/G2TXqb-QP",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/vTleFnr2r",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/DKLZFNJXw",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/ncsu6rxGC",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/hkEewthVn",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/23PL5zlTP",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/jdipSvxGl",
  },
  // {
  //   type: "iframe",
  //   url: "https://editor.p5js.org/shibomb/full/5UXwLgtlq",
  // },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/QYGEpof9-",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/GocLympMX",
  },
  // {
  //   type: "iframe",
  //   url: "https://editor.p5js.org/shibomb/full/6LdDTx1em",
  // },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/Zd2cPfeU0",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/ghN70NJ3u",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/_1qYAmz74",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/GsJzLcqu1",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/-qN7wpzqd",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/KqCOnXZBCa",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/-l_A9OqIq",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/D6j4p4t2G",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/49Qww-uK7",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/c1lSfwwL8",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/Y8Liboymj",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/qVIjVFi1T",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/teX-2GHG6",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/usN92Le86",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/awXGI8_8J",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/pLM1QhApR",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/UkJlBtOO1",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/LuwNJA5J7",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/-3DOZ-zB_",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/33KTPLKZ9",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/IlLhbVz-3",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/L86AL_nbP",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/iC2vNNqD0",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/L5tBLEqgz",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/HQXf7pU15",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/rNA9qY-K6",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/NZS5e7lIj",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/JzLxPt2aj",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/g82K26zni",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/4Q8_0goBR",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/V0qirp0xU",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/yWASoc8Fx",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/xRWLNiIEn",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/7X7tN8xGz",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/YeEXd3lQ-",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/EnCw3w9QA",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/DPKx_WRlu",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/PtsIdk61l",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/F8krET83t",
  },
  // {
  //   type: "iframe",
  //   url: "https://editor.p5js.org/shibomb/full/AwWNhhPjI",
  // },
  // {
  //   type: "iframe",
  //   url: "https://editor.p5js.org/shibomb/full/EQQxTQoQf",
  // },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/CDCrTnqR-",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/FXqhZoFyu",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/EKFIHT7vX",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/oLyITgbp5",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/wAeOdfY19",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/EbT4OJnPb",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/6BlZDz-UA",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/xZdkTyK79",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/LUsPEVHa7",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/M1v8E64vq",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/UyllJxNVA",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/9XLd8p4zm",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/4nqedcJdZ",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/PzZuk3YG-",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/iE0YT0J5e",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/_vgxPWJWb",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/1e5OLSRPj",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/TbjI9XYHL",
  },
];
</script>
