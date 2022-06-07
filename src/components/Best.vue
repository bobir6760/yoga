<template>
  <div class="best">
    <div class="container">
      <div class="best-wrapper">
        <div class="best-wrapper-card">
          <div class="best-info">
            <div class="best-info__title">Practice <span>At Home </span></div>
            <div class="best__title">With the World’s Top YogaTeachers</div>
          </div>
          <div class="best-wrapper__subtitle">
            Stream hundreds of expertly led yoga & <br />meditation classes on
            any device. <br />Your free trial awaits. Cancel online anytime.
          </div>
          <div class="best-wrapper-btn">
            <button class="best__btn">Start your free trial</button>
          </div>
        </div>
        <div class="best-wrapper-item">
          <div class="best-wrapper__title">more than</div>
          <div class="best-item">
            <div class="best-item__number">200</div>
            <div class="best-item__title">classes</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Best",
};
</script>

<style lang="scss" scoped>
.best {
  padding: 100px 0px 50px 0px;
  display: flex;
  background-image: url("~@/assets/img/relax.png");
  background-size: cover;
  min-height: 80vh;
  width: 100%;
}
.best-wrapper {
  display: flex;
  gap: 50px;
  justify-content: space-between;
  margin-top: 80px;
}
.best-wrapper-card {
  display: flex;
  flex-direction: column;
  gap: 20px;
  margin-top: 50px;
  .best__btn {
    cursor: pointer;
    padding: 10px 45px;
    color: white;
    border: none;
    border-radius: 5px;
    background: #d3b10f;
    font-size: 15px;
  }
  .best__btn:active {
    background: #375b26;
  }
}
.best-info {
  .best-info__title {
    span {
      color: #375b26;
    }
    font-size: 40px;
  }
  .best__title {
    font-size: 18px;
    color: rgba(17, 39, 52, 0.7);
  }
}
.best-wrapper__subtitle {
  font-size: 15px;
  color: rgba(17, 39, 52, 0.7);
}
.best-wrapper-item {
  display: flex;
  align-items: center;
  gap: 5px;
  .best-wrapper__title {
    font-size: 30px;
    color: rgba(55, 91, 38, 0.41);
  }
}
.best-item {
  padding: 13px 15px 8px 15px;
  background: rgba(241, 212, 75, 0.4);
  border-radius: 50px;
  color: white;
  text-align: center;
  cursor: pointer;
  .best-item__number {
    font-size: 40px;
  }
}
.best-item:active {
  background: #375b26;
}
@media screen and (max-width: 768px) {
  .best-wrapper-item .best-wrapper__title {
    font-size: 25px;
  }
}
@media screen and (max-width: 576px) {
  .best-wrapper {
    flex-direction: column;
    text-align: center;
  }
  .best-wrapper-item {
    display: flex;
    justify-content: center;
  }
}
</style>
