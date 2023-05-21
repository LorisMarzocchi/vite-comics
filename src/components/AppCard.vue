<script>
export default {
  props: {
    price: String,
    series: String,
    type: String,
    thumb: String,
  },
};
</script>

<template>
  <div class="card">
    <img :src="thumb" alt="" />
    <p>{{ series }}</p>
  </div>
</template>

<style lang="scss" scoped>
.card {
  margin: 20px;
  width: calc((100% / 6) - 40px);
  height: 100%;
  p {
    color: white;
  }
}
img {
  width: 100%;
  height: 250px;
}
</style>
