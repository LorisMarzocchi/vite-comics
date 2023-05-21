<script>
import AppNavBar from "./AppNavBar.vue";

export default {
  data() {
    return {
      NavMenu: [
        {
          name: "CHARACTERS",
          src: "#",
        },
        {
          name: "COMICS",
          src: "#",
        },
        {
          name: "MOVIES",
          src: "#",
        },
        {
          name: "TV",
          src: "#",
        },
        {
          name: "GAMES",
          src: "#",
        },
        {
          name: "COLLECTIBLES",
          src: "#",
        },
        {
          name: "VIDEOS",
          src: "#",
        },
        {
          name: "FANS",
          src: "#",
        },
        {
          name: "NEWS",
          src: "#",
        },
        {
          name: "SHOP",
          src: "#",
        },
      ],
    };
  },
  components: {
    AppNavBar,
  },
};
</script>

<template>
  <header>
    <img src="../assets/img/dc-logo.png" alt="" />
    <AppNavBar :NavMenu="NavMenu" />
  </header>
</template>

<style lang="scss" scoped>
header {
  padding-inline: 100px;
  height: 120px;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: white;
}
img {
  height: 100px;
  width: 100px;
  background-color: white;
}
</style>
