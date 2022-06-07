<template>
  <div class="footer">
    <div class="container">
      <div class="footer-wrapper">
        <div class="footer-body-wrapper">
          <div class="footer-block-wrapper">
            <div class="footer-wrapper__title">Articles</div>
            <div class="footer-wrapper__subtitle">
              <p>Yoga</p>
              <p>Practice</p>
              <p>Meditation</p>
              <p>Yoga Therapy</p>
              <p>Pranayama</p>
              <p>Lifestyle</p>
              <p>Poses</p>
              <p>Tutorial</p>
            </div>
          </div>
          <div class="footer-block-wrapper">
            <div class="footer-wrapper__title">Classes</div>
            <div class="footer-wrapper__subtitle">
              <p>Beginner</p>
              <p>Hatha Yoga</p>
              <p>Prenatal</p>
              <p>Restorative</p>
              <p>Vinyasa</p>
            </div>
          </div>
          <div class="footer-block-wrapper">
            <div class="footer-wrapper__title">Courses</div>
            <div class="footer-wrapper__subtitle">
              <p>Featured</p>
              <p>Asana</p>
              <p>Ayurveda</p>
              <p>Conferences</p>
            </div>
          </div>
          <div class="footer-block-wrapper">
            <div class="footer-wrapper__title">Teachers</div>
            <div class="footer-wrapper__subtitle">
              <p>Chirtian Sell</p>
              <p>Rod Stryker</p>
              <p>Jim Bennitt</p>
              <p>Bernie Heron</p>
              <p>Jessica Stickler</p>
            </div>
          </div>
          <div class="footer-block-wrapper">
            <div class="footer-wrapper__title">About</div>
            <div class="footer-wrapper__subtitle">
              <p>Need help&</p>
              <p>Careers</p>
              <p>Privacy Policy</p>
              <p>Terms of Service</p>
            </div>
          </div>
        </div>
        <div class="footer-card-wrapper">
          <FooterCard
            v-for="(card, index) in cards"
            :key="index"
            :item="card"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import FooterCard from "@/components/FooterCard";
export default {
  name: "Footer",
  data() {
    return {
      cards: [
        {
          imgUrl: require("@/assets/img/whh1.svg"),
        },
        {
          imgUrl: require("@/assets/img/whh2.svg"),
        },
        {
          imgUrl: require("@/assets/img/whh3.svg"),
        },
        {
          imgUrl: require("@/assets/img/whh4.svg"),
        },
      ],
    };
  },
  components: {
    FooterCard,
  },
};
</script>

<style scoped lang="scss">
.footer {
  padding: 50px 0px;
  background: #112734;
}
.footer-wrapper {
  display: flex;
  flex-direction: column;
}
.footer-body-wrapper {
  display: flex;
  gap: 70px;
  .footer-block-wrapper {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .footer-wrapper__title {
    color: #f1d44b;
    font-size: 20px;
    font-weight: bold;
  }
  .footer-wrapper__subtitle {
    display: flex;
    flex-direction: column;
    gap: 20px;
    color: white;
    font-size: 18px;
  }
}
.footer-card-wrapper {
  display: flex;
  gap: 20px;
  justify-content: flex-end;
}
@media screen and (max-width: 992px) {
  .footer-body-wrapper {
    display: flex;
    gap: 50px;
    .footer-block-wrapper {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    .footer-wrapper__title {
      color: #f1d44b;
      font-size: 17px;
      font-weight: bold;
    }
    .footer-wrapper__subtitle {
      display: flex;
      flex-direction: column;
      gap: 10px;
      color: white;
      font-size: 14px;
    }
  }
  .footer-card-wrapper {
    gap: 7px;
  }
}
@media screen and (max-width: 768px) {
  .footer-body-wrapper {
    display: flex;
    gap: 30px;
    .footer-block-wrapper {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }
    .footer-wrapper__title {
      color: #f1d44b;
      font-size: 15px;
      font-weight: bold;
    }
    .footer-wrapper__subtitle {
      display: flex;
      flex-direction: column;
      gap: 10px;
      color: white;
      font-size: 11px;
    }
  }
  .footer-card-wrapper {
    gap: 0px;
  }
}
@media screen and (max-width: 576px) {
  .footer-wrapper {
    gap: 20px;
  }
  .footer-body-wrapper {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    .footer-block-wrapper {
      display: flex;
      flex-direction: column;
      gap: 20px;
    }
    .footer-wrapper__title {
      font-size: 18px;
    }
    .footer-wrapper__subtitle {
      display: flex;
      flex-direction: column;
      gap: 20px;
      font-size: 15px;
    }
  }
  .footer-card-wrapper {
    gap: 0px;
  }
  .footer-card-wrapper {
    display: flex;
    gap: 0px;
    justify-content: center;
  }
}
</style>
