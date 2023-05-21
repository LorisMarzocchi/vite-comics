<script>
export default {
  data() {
    return {
      NavMenu: [
        {
          name: CHARACTERS,
          src: "#",
          active: true,
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
};
</script>

<template>
  <ul>
    <li v-for="eleMenu in NavMenu" :key="eleMenu.name">
      <a href="#">{{ eleMenu.name }}</a>
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
