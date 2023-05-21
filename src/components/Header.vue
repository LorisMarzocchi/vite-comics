<script>
import NavBar from "./NavBar.vue";
export default {
  components: {
    NavBar,
  },
};
</script>

<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="" />
    <NavBar :menuElemnt="NavMenu" />
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
