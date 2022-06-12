<template>
  <div class="navbar-wrapper-item">
    <div class="navbar-wrapper__title">
      <span><p>Articles</p></span>
      <p>Classes</p>
      <p>Courses</p>
      <p>Teachers</p>
      <p>About</p>
    </div>
  </div>
</template>
<script>
export default {
  name: "navbar-card",
};
</script>
<style lang="scss" scoped>
.navbar-wrapper__title {
  display: flex;
  gap: 20px;
  font-weight: bold;
  span {
    color: #22B111;
  }
}
.navbar-wrapper__title p {
  cursor: pointer;
}
@media screen and (max-width: 1200px) {
  .navbar-wrapper__title {
    gap: 10px;
  }
}
@media screen and (max-width: 992px) {
  .navbar-wrapper__title {
    font-size: 12px;
  }
}
@media screen and (max-width: 768px) {
  .navbar-wrapper__title {
    font-size: 18px;
  }
}
@media screen and (max-width: 576px) {
  .navbar-wrapper__title {
    font-size: 15px;
  }
}
</style>
