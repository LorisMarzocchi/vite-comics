<script>
import AppNavBar from "./AppNavBar.vue";

export default {
  data() {
    return {
      logoImgName: "dc-logo.png",
    };
  },
  methods: {
    getImagePath(img) {
      return new URL(`../assets/img/${img}`, import.meta.url).href;
    },
  },
  components: {
    AppNavBar,
  },
};
</script>

<template>
  <header>
    <img :src="getImagePath(logoImgName)" alt="" />
    <AppNavBar />
  </header>
</template>

<style scoped>
header {
  max-width: 1000px;
  height: 120px;
  margin: auto;
}
img {
  height: 100px;
  width: 100px;
  background-color: white;
}
</style>
