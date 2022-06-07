<template>
  <div class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <div class="navbar-card">
          <div class="navbar-card__image">
            <img src="@/assets/img/Group 1.png" alt="" />
          </div>
          <div class="navbar-card__title"><span>Yoga</span> International</div>
        </div>
        <div class="navbar-wrapper-block">
          <NavbarCard />
        </div>
        <div class="navbar-wrapper-text">
          <div class="navbar-image">
            <img src="@/assets/img/Lupa.png" alt="" />
          </div>
          <div class="navbar-wrapper__btn">
            <button class="navbar-wrapper-btn">Sign In</button>
          </div>
          <div class="navbar-wrapper__btn">
            <button class="navbar-btn">Start your free trial</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavbarCard from "@/components/NavbarCard";
export default {
  name: "Navbar",
  components: {
    NavbarCard,
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  padding: 50px 0px;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
}
.navbar-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.navbar-card {
  display: flex;
  align-items: center;
  gap: 5px;
  .navbar-card__image img {
    width: 100%;
  }
  .navbar-card__title {
    font-size: 22px;
    font-weight: bold;
    span {
      color: #375b26;
    }
  }
}
.navbar-wrapper-text {
  display: flex;
  align-items: center;
  gap: 20px;
  .navbar-image img {
    width: 100%;
  }
}
.navbar-wrapper-btn {
  padding: 6px;
  border-radius: 5px;
  font-weight: bold;
  cursor: pointer;
}
.navbar-wrapper-btn:active {
  background: #d3b10f;
  border: none;
}
.navbar-btn {
  padding: 7px;
  color: white;
  background: #d3b10f;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
.navbar-btn:active {
  background: #375b26;
}
@media screen and (max-width: 992px) {
  .navbar-btn {
    font-size: 10px;
  }
  .navbar-wrapper-btn {
    font-size: 10px;
  }
  .navbar-wrapper-text {
    gap: 10px;
  }
}
@media screen and (max-width: 768px) {
  .navbar-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
  }
  .navbar-btn {
    font-size: 15px;
  }
  .navbar-wrapper-btn {
    font-size: 15px;
  }
  .navbar-wrapper-text {
    gap: 20px;
  }
}
</style>
