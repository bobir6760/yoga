<template>
  <div class="challenge">
    <div class="container">
      <div class="challenge-wrapper">
        <div class="challenge-wrapper-card">
          <div class="challenge-wrapper__title">
            Challenge <span>Yourself</span>
          </div>
          <div class="challenge-wrapper__subtitle">
            Take your practice to the next level with our on-going yoga
            challenges
          </div>
        </div>
        <div class="challenge-wrapper-item">
          <div class="challenge-wrapper__image">
            <img src="@/assets/img/yoga3.png" alt="" />
          </div>
          <div class="challenge-wrapper__image">
            <img src="@/assets/img/yoga2.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Challenge",
};
</script>

<style lang="scss" scoped>
.challenge {
  padding: 50px 0px;
}
.challenge-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
}
.challenge-wrapper-card {
  display: flex;
  flex-direction: column;
  gap: 30px;
  .challenge-wrapper__title {
    font-size: 40px;
    cursor: pointer;
    span {
      color: #22B111;
    }
  }
  .challenge-wrapper__title:hover {
    text-decoration: underline;
  }
  .challenge-wrapper__subtitle {
    font-size: 18px;
    color: rgba(17, 39, 52, 0.7);
    cursor: pointer;
  }
}
.challenge-wrapper-item {
  display: flex;
  gap: 30px;
  .challenge-wrapper__image img {
    width: 100%;
    cursor: pointer;
  }
  .challenge-wrapper__image {
    display: flex;
    overflow: hidden;
    border-radius: 10px;
  }
}
@media screen and (max-width: 992px) {
  .challenge-wrapper-card {
    gap: 15px;
    .challenge-wrapper__title {
      font-size: 35px;
    }
  }
}
@media screen and (max-width: 992px) {
  .challenge-wrapper-card {
    gap: 15px;
    .challenge-wrapper__title {
      font-size: 30px;
    }
    .challenge-wrapper__subtitle {
      font-size: 14px;
    }
  }
}
@media screen and (max-width: 992px) {
  .challenge-wrapper-item {
    gap: 20px;
    flex-direction: column;
  }
}
</style>
