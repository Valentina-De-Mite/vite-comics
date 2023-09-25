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
  <div class="comic_card col-sm-2 col-2">
    <div class="card_container">
      <img class="w-75 comic" :src="thumb" alt="" />
    </div>
    <a class="mt-5 text-decoration-none link">{{ series }}</a>
    <p>{{ price }}</p>
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

.comic {
  height: 200px;
}
</style>
