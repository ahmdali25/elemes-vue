<template>
  <nav class="container header pt-3">
    <div class="row align-items-center">
      <div class="col-3">
        <img src="../assets/images/logo.png" alt="Logo" />
      </div>
      <div class="col-5 mt-3">
        <ul class="list">
          <li><router-link class="nav" to="/">Home</router-link></li>
          <li><router-link class="nav" to="/about">About</router-link></li>
          <li>
            <span class="hot">Hot</span>
            <router-link class="nav" to="/promotions">Promotions</router-link>
          </li>
          <li><router-link class="nav" to="/blogs">Blogs</router-link></li>
          <li>
            <router-link class="nav" to="/contact-us">Contact Us</router-link>
          </li>
        </ul>
      </div>
      <div class="col-4">
        <div class="nav-wrapper">
          <span class="nav">Masuk</span>
          <BaseButton
            name="Daftar Sekarang"
            :isPrimary="true"
            :hasShadow="false"
          />
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import BaseButton from "../components/BaseButton.vue";

export default {
  name: "BaseNavbar",
  components: { BaseButton },
};
</script>

<style scoped>
.header {
  position: relative;
  z-index: 1;
}

.list {
  list-style: none;
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 32px;
}

.list .nav {
  font-weight: 500;
  font-size: 14px;
  color: #757575;
  text-decoration: none;
}

.list .hot {
  position: absolute;
  top: -42%;
  right: 37.5%;
  background: #e7462d;
  width: 36px;
  height: 19px;
  border-radius: 8px;
  font-weight: 700;
  font-size: 8px;
  text-transform: uppercase;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #ffffff;
}

.nav-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 24px;
}

.nav {
  font-weight: 500;
  font-size: 14px;
  color: #333333;
}
</style>
