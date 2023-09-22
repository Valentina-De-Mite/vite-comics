<script>
import AppLogo from "./components/AppLogo.vue";
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  data() {
    return {};
  },

  components: {
    AppLogo,
    AppHeader,
    AppMain,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use "/node_modules/bootstrap/scss/bootstrap";
</style>
