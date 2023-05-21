<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppNavBar from "./components/AppNavBar.vue";

export default { components: { AppHeader, AppMain, AppFooter, AppNavBar } };
</script>

<template>
  <AppHeader>
    <AppNavBar></AppNavBar>
  </AppHeader>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use "./assets/style/general.scss" as *;
</style>
