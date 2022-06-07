<template>
  <div class="time">
    <div class="container">
      <div class="time-wrapper">
        <div class="time-wrapper-card">
          <div class="time-wrapper__title">
            At Home Or On-The-Go <br /><span>Always On Your Time</span>
          </div>
        </div>
        <div class="time-wrapper-item">
          <div class="time-wrapper__image">
            <img src="@/assets/img/IMG4.png" alt="" />
          </div>
          <div class="time-wrapper-block">
            <div class="time-block__title">
              Customize your membership and grow your practice <br />by choosing
              from our expansive library of classes, courses, <br />and
              articles.
            </div>
            <div class="time-item">
              <div class="time-image">
                <img src="@/assets/img/IMG9.png" alt="" />
              </div>
              <div class="time-card-block">
                <div class="time-item-card">
                  <div class="time-item-body">
                    <div class="time-body-image">
                      <img src="@/assets/img/IMG6.svg" alt="" />
                    </div>
                    <div class="time-item__title">Hatha yoga</div>
                  </div>
                  <div class="time-item__subtitle">Level 2</div>
                </div>
                <div class="time-item__text">Love Your (Warrior) Feet</div>
              </div>
              <div class="time-card-body">
                <div class="time-body-card">
                  <div class="time-body__image">
                    <img src="@/assets/img/IMG7.png" alt="" />
                  </div>
                  <div class="time-body__title">Noah Maze</div>
                </div>
                <div class="time-body-card">
                  <div class="time-body__image">
                    <img src="@/assets/img/IMG8.png" alt="" />
                  </div>
                  <div class="time-body__title">45 min</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Time",
};
</script>

<style lang="scss" scoped>
.time {
  padding: 50px 0px;
}
.time-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
  text-align: center;
}
.time-wrapper-card {
  display: flex;
  flex-direction: column;
  .time-wrapper__title {
    font-size: 35px;
    span {
      color: #375b26;
    }
  }
}
.time-wrapper-item {
  display: flex;
  gap: 50px;
  text-align: start;
  justify-content: center;
  .time-wrapper__image img {
    width: 100%;
  }
  .time-wrapper__image {
    display: flex;
    overflow: hidden;
    border-radius: 15px;
  }
}
.time-wrapper-block {
  display: flex;
  flex-direction: column;
  gap: 30px;
  border-radius: 15px;
  .time-block__title {
    color: rgba(17, 39, 52, 0.7);
  }
}
.time-item {
  background: white;
  display: flex;
  flex-direction: column;
  gap: 10px;
  border-radius: 15px;
  .time-image img {
    width: 100%;
  }
  .time-image {
    display: flex;
    overflow: hidden;
    border-radius: 15px;
  }
}
.time-item-body {
  display: flex;
  gap: 5px;
  align-items: center;
  .time-item__title {
    font-size: 22px;
  }
  .time-body-image img {
    width: 100%;
  }
  .time-body-image {
    padding: 6px 7px 4px 8px;
    background: #f1d44b;
    border-radius: 30px;
  }
}
.time-item-card {
  padding: 0px 10;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.time-card-block {
  display: flex;
  flex-direction: column;
  gap: 15px;
  padding: 0px 15px;
}
.time-card-body {
  display: flex;
  justify-content: space-between;
  padding: 15px;
  .time-body-card {
    display: flex;
    gap: 10px;
    align-items: center;
  }
}
@media screen and (max-width: 992px) {
  .time-wrapper-block {
    gap: 20px;
    .time-block__title {
      font-size: 15px;
      color: rgba(17, 39, 52, 0.7);
    }
  }
  .time-wrapper-item {
    gap: 20px;
  }
  .time-wrapper {
    gap: 30px;
  }
}
@media screen and (max-width: 992px) {
  .time-wrapper-item {
    flex-direction: column;
  }
  .time-wrapper-block {
    .time-block__title {
      text-align: center;
      font-size: 20px;
    }
  }
  .time-wrapper-card {
    .time-wrapper__title {
      font-size: 30px;
    }
  }
}
@media screen and (max-width: 576px) {
  .time-wrapper-card {
    .time-wrapper__title {
      font-size: 28px;
    }
  }
  .time-wrapper-block {
    .time-block__title {
      font-size: 12px;
    }
  }
  .time-item-body .time-item__title {
    font-size: 18px;
  }
  .time-item__text {
    font-size: 15px;
  }
}
</style>
