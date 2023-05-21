<script>
export default {
  props: {
    NavMenu: Array,
  },
};
</script>

<template>
  <ul>
    <li v-for="eleMenu in NavMenu" :key="eleMenu.name">
      <a href="#">{{ eleMenu.name }}</a>
    </li>
  </ul>
</template>

<style lang="scss" scoped>
ul {
  display: flex;
  justify-content: center;
  list-style: none;
  gap: 1rem;
}
a {
  text-decoration: none;
}
/* li a::after {
  content: "";
  display: block;
  width: 50px;
  height: 5px;
  background-color: #0282f9;
  position: absolute;
  top: 71px;
  left: 49px;
} */
</style>
