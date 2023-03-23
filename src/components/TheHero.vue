<template>
  <section class="container hero-section">
    <div class="row align-items-center">
      <div class="col-5">
        <h1 class="hero-heading">Good Food Us Good Mood</h1>
        <p class="hero-paragraph mt-4">
          I would think that conserving our natural resources should be a
          conservative position: Not to waste food, and not to throw away a lot
          of the food that we buy.
        </p>
        <div class="row mt-4">
          <div class="col-5 mr-2">
            <BaseButton
              name="Daftar Sekarang"
              :isPrimary="true"
              :hasShadow="true"
            />
          </div>
          <div class="col-5 ml-n5">
            <BaseButton name="About Us" :isPrimary="false" :hasShadow="false" />
          </div>
        </div>
      </div>
      <div class="col-7">
        <div class="row justify-content-end">
          <img class="hero-image" src="../assets/images/food.png" alt="Food" />
        </div>
        <div class="card-profile">
          <div class="row">
            <div class="col-3">
              <img
                class="card-profile-image"
                src="../assets/images/food.png"
                alt="Food"
              />
            </div>
            <div class="col">
              <h6 class="card-profile-title">Green Salad Tomato</h6>
              <p class="card-profile-detail">Tomato</p>
              <BaseStarIcon :isFilled="3" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import BaseStarIcon from "../components/BaseStarIcon.vue";
import BaseButton from "../components/BaseButton.vue";

export default {
  name: "TheHero",
  components: { BaseStarIcon, BaseButton },
};
</script>

<style scoped>
.hero-section:before {
  content: " ";
  display: block;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  opacity: 0.04;
  background: url("../assets/images/hero.png");
  background-repeat: no-repeat;
  background-position: 100% 0;
  background-size: cover;
}

.hero-section {
  margin-top: 30px;
}

.hero-heading {
  font-weight: 500;
  font-size: 64px;
  line-height: 64px;
  color: #8bac3e;
}

.hero-paragraph {
  font-weight: 400;
  font-size: 18px;
  line-height: 29px;
  color: #757575;
}

.hero-image {
  background: #f7f7f7;
  border-radius: 999px;
  padding: 50px;
}

.card-profile {
  position: absolute;
  z-index: 10;
  top: 78%;
  right: 44%;
  background: rgba(255, 255, 255, 0.74);
  box-shadow: 0px 11px 39px rgba(0, 0, 0, 0.07);
  border-radius: 17px;
  width: 292px;
  height: 93px;
  padding: 18px 23px;
}

.card-profile-image {
  width: 53px;
  height: 53px;
}

.card-profile-title {
  font-weight: 600;
  font-size: 14px;
}

.card-profile-detail {
  margin-top: -5px;
  font-weight: 400;
  font-size: 12px;
  color: #757575;
}
</style>
