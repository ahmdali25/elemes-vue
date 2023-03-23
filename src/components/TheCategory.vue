<template>
  <section class="container category-section">
    <div class="row">
      <div class="col">
        <h1 class="category-title">
          Browse Our Category <br />
          <span>Receipt</span>
        </h1>
      </div>
    </div>
    <div class="food-wrapper">
      <div v-for="(food, index) in foods" :key="index">
        <div class="food-card" :style="{ backgroundColor: food.color }">
          <div class="bg-wrapper"></div>
          <img
            class="food-image"
            :src="require(`../assets/images/${food.name}.svg`)"
            :alt="food.name"
          />
          <div class="food-detail">
            <p class="food-name text-center">{{ food.name }}</p>
            <p class="food-total text-center">{{ food.total }} items</p>
          </div>
        </div>
      </div>
    </div>
    <div class="nav-wrapper">
      <div class="button button--state-primary">
        <div class="button-detail">
          <div class="icon-circle">
            <b-icon
              icon="chevron-left"
              font-scale="1.5"
              style="color: #8bac3e"
            ></b-icon>
          </div>
          <span>Prev</span>
        </div>
      </div>
      <div class="button button--state-primary">
        <div class="button-detail">
          <div class="icon-circle">
            <b-icon
              icon="chevron-right"
              font-scale="1.5"
              style="color: #8bac3e"
            ></b-icon>
          </div>
          <span>Next</span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TheCategory",
  data: () => ({
    foods: [
      { id: 1, name: "cupcake", total: 22, color: "#F0FEEB" },
      { id: 2, name: "pizza", total: 25, color: "#E4F2F4" },
      { id: 3, name: "kebab", total: 12, color: "#EAEEFA" },
      { id: 4, name: "salmon", total: 22, color: "#F9EEF3" },
      { id: 5, name: "doughnut", total: 11, color: "#F3F7D9" },
    ],
  }),
};
</script>

<style scoped>
.category-section {
  padding: 100px 0;
}

.category-title {
  font-family: "Rubik";
  font-weight: 500;
  font-size: 38px;
  color: #333333;
}

.category-title span {
  color: #8bac3e;
}

.food-wrapper {
  margin-top: 40px;
  display: flex;
  flex-direction: row;
  gap: 11px;
  height: 180px;
}

.food-card {
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 30px 81px;
  width: 230px;
  height: 175px;
  border-radius: 8px;
}

.food-card:hover {
  height: 195px;
}

.food-name {
  margin-top: 21px;
  font-weight: 500;
  font-size: 16px;
  color: #333333;
  text-transform: capitalize;
}

.food-total {
  margin-top: -18px;
  font-weight: 400;
  font-size: 14px;
  color: #333333;
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

.food-image {
  z-index: 10;
}

.food-detail {
  z-index: 10;
}

.nav-wrapper {
  padding: 40px 0;
  display: flex;
  flex-direction: row;
  justify-content: end;
  gap: 10px;
}

.button {
  background: #f2f2f2;
  color: #333333;
  font-weight: 500;
  font-size: 14px;
  padding: 9px 13px;
  width: 113px;
  height: 50px;
  border-radius: 100px;
  border: none;
  cursor: pointer;
}

.button--state-primary {
  background: #8bac3e;
  color: #ffffff;
}

.button-detail {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 10px;
}

.icon-circle {
  width: 33px;
  height: 33px;
  background: #ffffff;
  border-radius: 100px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.button span {
  text-transform: uppercase;
  font-weight: 500;
  font-size: 16px;
}
</style>
