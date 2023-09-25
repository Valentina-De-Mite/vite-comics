<script>
import CardComponent from "./CardComponent.vue";
import Cards from "../assets/card.js";
export default {
  name: "AppMain",

  components: {
    CardComponent,
  },

  data() {
    return {
      Cards,
    };
  },
};
</script>

<template>
  <div class="jumbotron py-5"></div>

  <div class="blue fs-4 text-light py-3">
    <div
      class="container row m-auto justify-content-between align-items-center"
    >
      <CardComponent
        v-for="card in Cards"
        :image_src="card.image_source"
        :description="card.description"
      ></CardComponent>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.black {
  background-color: black;
  color: white;
}
.blue {
  background-color: #68bafc;
}

.jumbotron {
  background-image: url(../assets/img/jumbotron.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 50vh;
}
</style>
