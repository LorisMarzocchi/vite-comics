<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import Items from "./components/Items.vue";

export default {
  components: {
    Header,
    Main,
    Footer,
    Items,
  },
};
</script>

<template>
  <Header></Header>
  <Main>
    <Items></Items>
  </Main>
  <Footer></Footer>
</template>

<style lang="scss">
@use "./assets/style/general.scss" as *;
</style>
