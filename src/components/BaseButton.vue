<template>
  <button
    class="button"
    :class="{
      'button--state-primary': isPrimary,
      'button--state-shadow': hasShadow,
    }"
  >
    {{ name }}
  </button>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      required: true,
    },
    isPrimary: {
      type: Boolean,
    },
    hasShadow: {
      type: Boolean,
    },
  },
};
</script>

<style scoped>
.button {
  background: #f2f2f2;
  color: #333333;
  font-weight: 500;
  font-size: 14px;
  padding: 10px 18px;
  height: 42px;
  border-radius: 100px;
  border: none;
}

.button--state-primary {
  background: #8bac3e;
  color: #ffffff;
}

.button--state-shadow {
  box-shadow: 0px 8px 32px rgba(102, 107, 226, 0.35);
}
</style>
