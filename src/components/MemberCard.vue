<template>
  <div class="member-item">
    <div class="member-item__image">
      <img :src="item.imgUrl" alt="" />
    </div>
    <div class="member-item__title">{{ item.title }}</div>
    <div class="member-item__subtitle">{{ item.subtitle }}</div>
  </div>
</template>
<script>
export default {
  name: "member-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style scoped lang="scss">
.member-item {
  padding: 16px;
  border-radius: 5px;
  background-color: white;
  display: flex;
  flex-direction: column;
  gap: 15px;
}
.member-item__title {
  font-size: 27px;
  color: #b6990f;
  cursor: pointer;
}
.member-item__title:hover {
  text-decoration: underline gray;
}
.member-item__image img {
  width: 100%;
  cursor: pointer;
}
.member-item__subtitle {
  font-size: 15px;
  cursor: pointer;
}
@media screen and (max-width: 992px) {
  .member-item {
    padding: 30px 5px;
    border-radius: 5px;
    background-color: white;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  .member-item__title {
    font-size: 20px;
    color: #b6990f;
  }
  .member-item__image img {
    width: 100%;
  }
  .member-item__subtitle {
    font-size: 12px;
  }
}
@media screen and (max-width: 768px) {
  .member-item {
    padding: 30px 5px;
    border-radius: 5px;
    background-color: white;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  .member-item__title {
    font-size: 17px;
    color: #b6990f;
  }
  .member-item__image img {
    width: 100%;
  }
  .member-item__subtitle {
    font-size: 10px;
  }
}
@media screen and (max-width: 576px) {
  .member-item {
    padding: 30px 5px;
    border-radius: 5px;
    background-color: white;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  .member-item__title {
    font-size: 22px;
    color: #b6990f;
  }
  .member-item__image img {
    width: 100%;
  }
  .member-item__subtitle {
    font-size: 15px;
  }
}
</style>
