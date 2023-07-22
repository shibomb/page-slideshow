# base

## Project setup

```
# yarn
yarn

# npm
npm install

# pnpm
pnpm install
```

## Edit slide urls

edit src/views/Slideshow.vue

```javascript
const contents = [
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/k0q_SyCyy",
  },
  {
    type: "iframe",
    url: "https://editor.p5js.org/shibomb/full/G2TXqb-QP",
  },
  {
    type: "image",
    url: "https://something/image/example.jpg",
  },
  :
```

### Compiles and hot-reloads for development

```
# yarn
yarn dev

# npm
npm run dev

# pnpm
pnpm dev
```

### Compiles and minifies for production

```
# yarn
yarn build

# npm
npm run build

# pnpm
pnpm build
```

### Lints and fixes files

```
# yarn
yarn lint

# npm
npm run lint

# pnpm
pnpm lint
```

### Customize configuration

See [Configuration Reference](https://vitejs.dev/config/).
