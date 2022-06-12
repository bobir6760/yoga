<template>
  <div class="practice-card-wrapper">
    <div class="practice-wrapper__image">
      <img :src="item.imgUrl" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "practice-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style lang="scss" scoped>
.practice-card-wrapper {
  display: flex;
  justify-content: center;
}
.practice-wrapper__image img {
  width: 100%;
  border-radius: 120px;
  cursor: pointer;
}
.practice-wrapper__image {
  display: flex;
  gap: 20px;
  cursor: pointer;
}
</style>
