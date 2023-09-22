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
  <div class="container">
    <nav class="navbar navbar-expand justify-content-between">
      <AppLogo></AppLogo>
      <div class="nav navbar-nav h-100">
        <a class="nav-item nav-link bordo" href="#" aria-current="page"
          >CHARACTERS</a
        >
        <a class="nav-item nav-link bordo" href="#">COMICS</a>
        <a class="nav-item nav-link bordo" href="#">MOVIES</a>
        <a class="nav-item nav-link bordo" href="#">TV</a>
        <a class="nav-item nav-link bordo" href="#">COLLECTIBLES</a>
        <a class="nav-item nav-link bordo" href="#">VIDEOS</a>
        <a class="nav-item nav-link bordo" href="#">FANS</a>
        <a class="nav-item nav-link bordo" href="#">NEWS</a>
        <a class="nav-item nav-link bordo" href="#">SHOP</a>
      </div>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
.bordo:hover {
  border-bottom: 5px solid rgb(38, 77, 207) !important;
}
a {
  height: 100%;
}
</style>
