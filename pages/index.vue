<template>
  <div class="mx-2 mt-3">
    <b-card-group deck class="card-deck">
      <b-card
        v-for="sign in signs"
        :key="sign.title"
        img-src="~/assets/200.png"
        :img-alt="sign.title"
        img-bottom
      >
        <!-- style="max-width: 20rem;" -->
        <b-card-text>
          <p>> {{ sign.title }}</p>
        </b-card-text>
      </b-card>
    </b-card-group>

    <!-- Popular -->

    <div class="row mx-2 mt-5">
      <div class="col-3">
        <Carousel />
      </div>
      <div class="col-9">
        <h5>Popular Custom Templates</h5>
        <p>
          > Our affordable custom products feature 3M inks and films. The
          overlaminate protects signs for over 10 years.
        </p>
        <b-card-group deck class="card-deck">
          <b-card
            v-for="product in popularProducts"
            :key="product.title"
            :img-src="product.img"
            :img-alt="product.title"
            img-bottom
          >
            <!-- style="max-width: 20rem;" -->
            <b-card-text>
              <p>> {{ product.title }}</p>
            </b-card-text>
          </b-card>
        </b-card-group>
      </div>
    </div>
  </div>
</template>

<script>
// import ProductCard from "~/components/ProductCard";
import Carousel from "~/components/Carousel";

export default {
  components: {
    Carousel
  },
  computed: {
    signs() {
      return [
        {
          title: "Social Distancing Signs",
          img: "200.png"
        },
        {
          title: "Social Distancing Signs",
          img: "200.png"
        },
        {
          title: "Social Distancing Signs",
          img: "200.png"
        },
        {
          title: "Social Distancing Signs",
          img: "200.png"
        },
        {
          title: "Social Distancing Signs",
          img: "200.png"
        },
        {
          title: "Social Distancing Signs",
          img: "200.png"
        }
      ];
    },
    popularProducts() {
      return [
        {
          title: "Danger",
          img:
            "https://images.mysafetysign.com/img/dp/csd/custom-danger-ansi-signs-120.jpg"
        },
        {
          title: "Danger",
          img:
            "https://images.mysafetysign.com/img/dp/csd/custom-danger-ansi-signs-120.jpg"
        },
        {
          title: "Danger",
          img:
            "https://images.mysafetysign.com/img/dp/csd/custom-danger-ansi-signs-120.jpg"
        },
        {
          title: "Danger",
          img:
            "https://images.mysafetysign.com/img/dp/csd/custom-danger-ansi-signs-120.jpg"
        }
      ];
    }
  }
};
</script>

<style>
/* .container_middle {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
} */
.card-deck {
  color: blue;
  font-weight: 700;
}
</style>
