<template>
  <h1 class="category-title">
    Browse Our {{ title }} <br />
    <span>Receipt</span>
  </h1>
</template>

<script>
export default {
  name: "BaseSectionTitle",
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.category-title {
  font-weight: 500;
  font-size: 38px;
  color: #333333;
}

.category-title span {
  color: #8bac3e;
}
</style>
