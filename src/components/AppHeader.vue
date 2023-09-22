<script>
import AppLogo from "./AppLogo.vue";
export default {
  name: "AppHeader",
  components: {
    AppLogo,
  },
};
</script>

<template>
  <nav class="navbar navbar-expand justify-content-evenly">
    <AppLogo></AppLogo>
    <div class="nav navbar-nav">
      <a class="nav-item nav-link" href="#" aria-current="page">CHARACTERS</a>
      <a class="nav-item nav-link" href="#">COMICS</a>
      <a class="nav-item nav-link active-item" href="#">MOVIES</a>
      <a class="nav-item nav-link" href="#">TV</a>
      <a class="nav-item nav-link" href="#">COLLECTIBLES</a>
      <a class="nav-item nav-link" href="#">VIDEOS</a>
      <a class="nav-item nav-link" href="#">FANS</a>
      <a class="nav-item nav-link" href="#">NEWS</a>
      <a class="nav-item nav-link" href="#">SHOP</a>
    </div>
  </nav>
</template>

<style lang="scss" scoped></style>
