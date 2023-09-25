<script>
export default {
  name: "ComicComponent",
  props: {
    thumb: String,
    series: String,
    price: Number,
  },
};
</script>

<template>
  <div class="col-2">
    <div class="comic_card">
      <img class="w-25" :src="thumb" alt="" />
      <p>{{ series }}</p>
      <p>{{ price }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
a {
  color: white !important;
}
.link:hover,
.tb:hover {
  text-decoration: underline !important;
}
</style>
