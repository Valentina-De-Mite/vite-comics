<script>
import ComicComponent from "./ComicComponent.vue";
import CardComponent from "./CardComponent.vue";
import Cards from "../assets/card.js";
import comics from "../assets/comics.js";
export default {
  name: "AppMain",

  components: {
    CardComponent,
    ComicComponent,
  },

  data() {
    return {
      comics,
      Cards,
    };
  },
};
</script>

<template>
  <div class="jumbotron py-5"></div>

  <div class="black">
    <div class="container series py-5 text-center">
      <div class="blue popup py-1 px-3 fw-medium text-center text-light fs-4">
        CURRENT SERIES
      </div>
      <div class="row-cols-sm-6 row">
        <ComicComponent
          v-for="comic in comics"
          :thumb="comic.thumb"
          :series="comic.series"
          :price="comic.price"
        >
        </ComicComponent>
      </div>

      <button class="btn btn-primary py-2 px-5 fs-5 mt-4 fw-medium">
        LOAD MORE
      </button>
    </div>
  </div>

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
  background-color: rgb(27, 27, 27);
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

.series {
  position: relative;
}

.popup {
  position: absolute;
  top: -25px;
  left: 25px;
}
</style>
