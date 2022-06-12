<template>
  <div class="from">
    <div class="container">
      <div class="from-wrapper">
        <div class="from-card-wrapper">
          <div class="from-wrapper__title">
            <span>Empowerment </span> <br />comes from within
          </div>
          <div class="from-wrapper__subtitle">
            Be part of a community of expert <br />yoga practitioners and
            members alike
          </div>
          <div class="from-wrapper-btn">
            <button class="from-btn">Start your journey</button>
          </div>
        </div>
        <div class="from-item-wrapper">
          <div class="from-wrapper__image">
            <img src="@/assets/img/choko.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "From",
};
</script>

<style lang="scss" scoped>
.from {
  padding: 50px 0px;
}
.from-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.from-card-wrapper {
  display: flex;
  flex-direction: column;
  gap: 30px;
  .from-wrapper__title {
    cursor: pointer;
    span {
      color: #375b26;
    }
    font-size: 60px;
  }
  .from-wrapper__subtitle {
    color: rgba(17, 39, 52, 0.7);
    font-size: 15px;
    cursor: pointer;
  }
}
.from-btn {
  cursor: pointer;
  padding: 15px 60px;
  font-size: 16px;
  color: white;
  background: #b6990f;
  border-radius: 5px;
  border: none;
}
.from-btn:active {
  background: #375b26;
}
.from-btn:hover {
  transition: 0.5s;
  box-shadow: inset 40px 0 0 0 black;
  border-radius: 15px;
  padding: 15px 40px 15px 80px;
}
.from-item-wrapper {
  display: flex;
}
.from-wrapper__image img {
  width: 100%;
  cursor: pointer;
}
@media screen and (max-width: 1200px) {
  .from-card-wrapper {
    display: flex;
    flex-direction: column;
    gap: 30px;
    .from-wrapper__title {
      span {
        color: #375b26;
      }
      font-size: 45px;
    }
    .from-wrapper__subtitle {
      font-size: 15px;
    }
  }
}
@media screen and (max-width: 992px) {
  .from-btn {
    cursor: pointer;
    padding: 12px 45px;
    font-size: 15px;
  }
  .from-card-wrapper {
    gap: 20px;
    .from-wrapper__title {
      font-size: 36px;
    }
    .from-wrapper__subtitle {
      font-size: 15px;
    }
  }
}
@media screen and (max-width: 768px) {
  .from-btn {
    cursor: pointer;
    padding: 12px 29px;
    font-size: 15px;
  }
  .from-card-wrapper {
    gap: 20px;
    .from-wrapper__title {
      font-size: 30px;
    }
    .from-wrapper__subtitle {
      font-size: 11px;
    }
  }
  .from-wrapper {
    gap: 20px;
  }
}
@media screen and (max-width: 576px) {
  .from-wrapper {
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 40px;
  }
  .from-card-wrapper {
    gap: 20px;
    .from-wrapper__title {
      font-size: 35px;
    }
    .from-wrapper__subtitle {
      font-size: 15px;
    }
  }
}
</style>
