<template>
  <ul class="star-list">
    <li v-for="(n, index) in 5" :key="index">
      <b-icon
        icon="star-fill"
        class="star-icon"
        :class="index < isFilled ? 'star-icon--filled' : ''"
      ></b-icon>
    </li>
  </ul>
</template>

<script>
export default {
  name: "BaseStarIcon",
  props: {
    isFilled: {
      type: Number,
      required: true,
    },
  },
};
</script>

<style scoped>
.star-list {
  margin-top: -20px;
  margin-left: -40px;
  list-style: none;
  display: flex;
  flex-direction: row;
  gap: 4px;
}

.star-icon {
  height: 10px;
  width: 10px;
  color: #c9c9c9;
}

.star-icon--filled {
  color: #ff8412;
}
</style>
