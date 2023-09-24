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
      <p class="ms-2 fs-6">{{ description }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
