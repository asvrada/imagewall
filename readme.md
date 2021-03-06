# vue image wall

[![Build Status](https://travis-ci.com/asvrada/vue-image-wall.svg?branch=master)](https://travis-ci.com/asvrada/vue-image-wall)

An interactive vue component that displays multiple images in a row.

By hovering mouse over one of the images, that image will expand in width.

[Demo](https://asvrada.github.io/rwby-imagewall-demo/) | [Demo Project](https://github.com/asvrada/rwby-imagewall-demo)

## Install

```
npm install vue-template-compiler --save-dev
npm install vue-image-wall
```

or

```
yarn add vue-template-compiler -D
yarn add vue-image-wall
```

## Usage
__FEATURES UNDER DEVELOPMENT__

1. Height is fixed to 250px, will be fixed
2. Will add ability to accept config (scale of image, animation duration, etc)

```
<template>
  <div id="app">
    <vue-image-wall :link-images="images"></vue-image-wall>
  </div>
</template>

<script>
  import VueImageWall from 'vue-image-wall';

  export default {
    name: 'app',
    components: { VueImageWall },
    data: function () {
      return {
        images: [
          '/assets/0.jpg',
          '/assets/1.jpg',
          '/assets/2.jpg',
          '/assets/3.jpg',
          '/assets/4.jpg'
        ],
      };
    },
  };
</script>

<style scoped>
</style>
```

| props | type | default value | note |
|-----|------|-------|------|
| link-images | `[String]` | (required) | Contains list of images that this component will display |

## How to Contribute

Any comment/issue/PR is welcome!

## TODO:
1. Add two interaction modes 
    1. macOS dock

## License

[MIT](https://opensource.org/licenses/MIT)
