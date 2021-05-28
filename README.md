# Animeta

Vue transition components powered by AnimeJS.

![](./public/Logo.png)

Demo：
Open in CodeSandbox: [vue-animeta](https://codesandbox.io/s/vue-animeta-jwd7i)

## 📦 Install

```bash
npm install vue-animeta
```

## 🔨 Usage

```jsx
<template>
  <animeta-transition
    :to="singleTo"
    :from="singleFrom"
    :options="singleOptions"
  >
    <div class="demo-box" v-if="!singleHidden"></div>
  </animeta-transition>
<template>
```

```js
import animeta from "vue-animeta";

export default {
  components: {
    ...animeta,
  },
  data() {
    return {
      // Single component demo
      singleTo: {
        scale: 1,
        opacity: 1,
        translateX: 0,
        translateY: 0,
        borderRadius: 15,
      },
      singleFrom: {
        scale: 0,
        opacity: 0,
        translateX: 300,
        translateY: 300,
        borderRadius: 100,
      },
      singleOptions: {
        duration: 750,
      },
      singleHidden: false,

      filterList: false,
      list: [1, 1, 1, 1, 1, 1, 1, 1],
    };
  },
};
```

## ⌨️ Development

Use Gitpod, a free online dev environment for GitHub.

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/cherislive/vue-animeta)

Or clone locally:

```bash
$ git clone https://github.com/cherislive/vue-animeta.git
$ cd vue-animeta
$ npm install
$ npm run serve
```
