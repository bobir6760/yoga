<template>
  <div class="footer-item-wrapper">
    <div class="footer-image">
      <img :src="item.imgUrl" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "footer-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style lang="scss" scoped>
.footer-image img {
  width: 100%;
  cursor: pointer;
}
@media screen and (max-width: 992px) {
  .footer-image img {
    width: 70%;
  }
}
@media screen and (max-width: 768px) {
  .footer-image img {
    width: 50%;
  }
  .footer-item-wrapper {
    text-align: center;
  }
}
</style>
