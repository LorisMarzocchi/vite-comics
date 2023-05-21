<script>
export default {
  data() {
    return {
      NavMenu: [
        {
          name: CHARACTERS,
          src: "#",
        },
        {
          name: COMICS,
          src: "#",
        },
        {
          name: MOVIES,
          src: "#",
        },
        {
          name: TV,
          src: "#",
        },
        {
          name: GAMES,
          src: "#",
        },
        {
          name: COLLECTIBLES,
          src: "#",
        },
        {
          name: VIDEOS,
          src: "#",
        },
        {
          name: FANS,
          src: "#",
        },
        {
          name: NEWS,
          src: "#",
        },
        {
          name: SHOP,
          src: "#",
        },
      ],
    };
  },
  props: {
    NavMenu: String,
  },
};
</script>

<template>
  <ul>
    <li v-for="menuElemet in NavMenu" :key="menuElemet.name">
      <a href="#">{{ menuElemet.name }}</a>
    </li>
  </ul>
</template>

<style>
.menu {
  height: 100%;
}
ul {
  display: flex;
  justify-content: center;
  gap: 0.5rem;
  list-style: none;
}
</style>
