<template>
  <main class="home">
    <TheHero />
    <TheCategory />
    <TheTrending />
  </main>
</template>

<script>
import TheHero from "../components/TheHero.vue";
import TheCategory from "../components/TheCategory.vue";
import TheTrending from "../components/TheTrending.vue";

export default {
  name: "HomeView",
  components: { TheHero, TheCategory, TheTrending },
};
</script>
