<template>
  <div id="app">
    <TheNavbar />
    <router-view />
    <TheFooter />
  </div>
</template>

<script>
import TheNavbar from "./components/TheNavbar.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  name: "App",
  components: { TheNavbar, TheFooter },
};
</script>

<style></style>
