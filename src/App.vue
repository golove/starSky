<template>
  <starsky :item="item" />
  <starsky :item="item1" />
  <starsky :item="item2" />
  <starsky :item="item3" />
</template>

<script>
import starsky from "./components/starsky.vue";

export default {
  name: "App",
  components: {
    starsky
  },
  data() {
    return {
      item: {
        count: 1000,
        size: 2,
        big: 3,
        scale: 1,
        blur: 0.4,
        color: {
          r: 20,
          g: 250,
          b: 210
        }
      },
      item1: {
        count: 1000,
        size: 2,
        big: 3,
        scale: 1,
        blur: 0.4,
        color: {
          r: 200,
          g: 150,
          b: 110
        }
      },
      item2: {
        count: 2000,
        size: 2,
        big: 1,
        scale: 1,
        blur: 1,
        color: {
          r: 200,
          g: 150,
          b: 110
        }
      },

      item3: {
        count: 30,
        size: 25,
        big: 8,
        scale: 6,
        blur: 18,
        color: {
          r: 220,
          g: 10,
          b: 10
        }
      }
    };
  }
};
</script>

<style>
body {
  width: 100vw;
  height: 100vh;
  color: #2c3e50;
  margin-top: 60px;
  background: radial-gradient(closest-side, #055383, #2b0b83, #04012e);
  z-index: -1;
}
</style>
