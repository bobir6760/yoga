<template>
  <div class="courses-item">
    <div class="courses-wrapper-block">
      <div class="courses-wrapper__image">
        <img src="@/assets/img/ptichka.svg" alt="" />
      </div>
      <div class="courses-wrapper__title">Courses</div>
      <div class="courses-wrapper__subtitle">$120</div>
    </div>
    <div class="courses-card">
      <div class="courses-card__title">{{ item.title }}</div>
    </div>
    <div class="courses-item-body">
      <div class="courses-wrapper-body">
        <div class="courses-item__image">
          <img :src="item.imgUrl" alt="" />
        </div>
        <div class="courses-item__title">Noah Maze</div>
      </div>
      <div class="courses-wrapper-body">
        <div class="courses-item__image">
          <img src="@/assets/img/Vector2.svg" alt="" />
        </div>
        <div class="courses-item__subtitle">45 min</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "courses-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.courses-item {
  display: flex;
  flex-direction: column;
  gap: 70px;
  padding: 20px;
  background-image: url("~@/assets/img/Component 6.png");
  overflow: hidden;
  border-radius: 5px;
}
.courses-item img {
  width: 100%;
}
.courses-wrapper-block {
  display: flex;
  align-items: center;
  gap: 3px;
  color: white;
}
.courses-card {
  display: flex;
  .courses-card__title {
    font-size: 25px;
    color: white;
    padding: 3px;
  }
}
.courses-wrapper-body {
  display: flex;
  align-items: center;
  .courses-item__image img {
    width: 100%;
  }
}
.courses-item__title {
  color: white;
}
.courses-item-body {
  display: flex;
  justify-content: space-between;
}
.courses-item__subtitle {
  color: white;
}
@media screen and (max-width: 576px) {
  .courses-card .courses-card__title {
    font-size: 21px;
  }
}
</style>
