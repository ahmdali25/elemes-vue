<template>
  <main class="home">
    <TheHero />
    <TheCategory />
  </main>
</template>

<script>
import TheHero from "../components/TheHero.vue";
import TheCategory from "../components/TheCategory.vue";

export default {
  name: "HomeView",
  components: { TheHero, TheCategory },
};
</script>
