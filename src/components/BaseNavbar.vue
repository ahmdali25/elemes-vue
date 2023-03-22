<template>
  <nav class="container pt-3">
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
        <div class="row align-items-center justify-content-center">
          <div class="col-2">
            <span class="nav">Masuk</span>
          </div>
          <div class="col-2">
            <button class="button button--state-primary">
              Daftar Sekarang
            </button>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "BaseNavbar",
};
</script>

<style scoped>
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

.nav {
  font-weight: 500;
  font-size: 14px;
  color: #333333;
}

.button {
  background: #f2f2f2;
  color: #333333;
  font-weight: 500;
  font-size: 14px;
  padding: 10px 18px;
  width: 147px;
  height: 42px;
  border-radius: 100px;
  border: none;
}

.button--state-primary {
  background: #8bac3e;
  color: #ffffff;
}
</style>
