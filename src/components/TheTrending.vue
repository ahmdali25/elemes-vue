<template>
  <section class="container trending-section">
    <div class="row">
      <div class="col">
        <BaseSectionTitle title="Trending" />
      </div>
    </div>
    <div class="row">
      <div class="col-3" v-for="(food, index) in trending" :key="index">
        <div class="card mt-4" :style="{ backgroundColor: food.color }">
          <div class="bg-wrapper"></div>
          <img class="image" :src="food.imageUrl" :alt="food.title" />
          <h4 class="food-title mt-3">{{ food.title }}</h4>
          <p class="food-category mb-4">{{ food.category }}</p>
          <BaseStarIcon :isFilled="food.rating" />
        </div>
      </div>
    </div>
    <div class="row justify-content-center mt-5">
      <BaseButton name="ALL Receipt" :isPrimary="true" :hasShadow="false" />
    </div>
  </section>
</template>

<script>
import BaseSectionTitle from "../components/BaseSectionTitle.vue";
import BaseStarIcon from "../components/BaseStarIcon.vue";
import BaseButton from "../components/BaseButton.vue";
import pizza_paperoni from "@/assets/images/pizza-paperoni.png";
import pizza_meat from "@/assets/images/pizza-meat.png";
import doner_kebab from "@/assets/images/doner-kebab.png";
import salmon_roll from "@/assets/images/salmon-roll.png";
import cupcake_choco from "@/assets/images/cupcake-choco.png";
import doughnut_milk from "@/assets/images/doughnut-milk.png";
import doughnut_unicorn from "@/assets/images/doughnut-unicorn.png";
import kathi_kebab from "@/assets/images/kathi-kebab.png";

export default {
  name: "TheTrending",
  components: { BaseSectionTitle, BaseStarIcon, BaseButton },
  data: () => ({
    trending: [
      {
        title: "Pizza Paperoni",
        category: "Pizza",
        rating: 4,
        imageUrl: pizza_paperoni,
        color: "#E6F3F5",
      },
      {
        title: "Pizza Meat",
        category: "Pizza",
        rating: 3,
        imageUrl: pizza_meat,
        color: "#E6F3F5",
      },
      {
        title: "Doner Kebab",
        category: "Kebab",
        rating: 5,
        imageUrl: doner_kebab,
        color: "#EAEEFA",
      },
      {
        title: "Salmon Roll",
        category: "Salmon",
        rating: 4,
        imageUrl: salmon_roll,
        color: "#F9EEF3",
      },
      {
        title: "Cupcake Choco",
        category: "Cupcake",
        rating: 4,
        imageUrl: cupcake_choco,
        color: "#F0FEEB",
      },
      {
        title: "Doughnut Milk",
        category: "Doughnut",
        rating: 5,
        imageUrl: doughnut_milk,
        color: "#F3F7D9",
      },
      {
        title: "Doughnut Unicorn",
        category: "Doughnut",
        rating: 4,
        imageUrl: doughnut_unicorn,
        color: "#F3F7D9",
      },
      {
        title: "Kathi Kebab",
        category: "Kebab",
        rating: 4,
        imageUrl: kathi_kebab,
        color: "#EAEEFA",
      },
    ],
  }),
};
</script>

<style scoped>
.trending-section {
  padding: 100px 0;
}

.card {
  background: #e6f3f5;
  box-shadow: 0px 11px 39px rgba(0, 0, 0, 0.07);
  border-radius: 17px;
  padding: 33px 20px;
}

.image {
  width: 118.15px;
  height: 120px;
  border-radius: 6px;
}

.food-title {
  font-weight: 500;
  font-size: 24px;
  color: #000000;
}

.food-category {
  font-weight: 500;
  font-size: 18px;
  line-height: 21px;
  color: #8bac3e;
}

.bg-wrapper {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}

.bg-wrapper:hover {
  background: url("../assets/images/hero.png");
  background-repeat: no-repeat;
  background-size: cover;
  opacity: 0.05;
  width: 100%;
  height: 100%;
  opacity: 0.09;
}
</style>
