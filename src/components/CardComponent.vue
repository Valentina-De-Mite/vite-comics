<script>
export default {
  name: "CardComponent",
  props: {
    image_src: String,
    description: String,
  },
};
</script>

<template>
  <div class="col-2 d-flex justify-content-center">
    <div class="text-center justify-content-center d-flex align-items-center">
      <img class="w-25" :src="image_src" alt="" />
      <a class="ms-2 fs-6 text-decoration-none link">{{ description }}</a>
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
