<template>
  <div class="practice">
    <div class="container">
      <div class="practice-wrapper">
        <div class="practice-body-wrapper">
          <div class="practice-wrapper__title">
            Practice with <span>confidence</span>
          </div>
          <div class="practice-wrapper__subtitle">
            Connect and study with 500+ expert teachers across yoga therapy,
            anatomy. meditation, and more. <br />The world’s most diverse yoga
            site.
          </div>
        </div>
        <div class="practice-card">
          <div class="practice-block-wrapper">
            <img src="@/assets/img/strelka1.svg" alt="" />
          </div>
          <div class="practice-item-wrapper">
            <PracticeCard
              v-for="(card, index) in cards"
              :key="index"
              :item="card"
            />
          </div>
          <div class="practice-block-wrapper">
            <img src="@/assets/img/strelka2.svg" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import PracticeCard from "@/components/PracticeCard";
export default {
  name: "Practice",
  data() {
    return {
      cards: [
        {
          imgUrl: require("@/assets/img/kartinka1.jpg"),
        },
        {
          imgUrl: require("@/assets/img/kartinka3.jpg"),
        },
        {
          imgUrl: require("@/assets/img/kartinka3.jpg"),
        },
        {
          imgUrl: require("@/assets/img/kartinka4.jpg"),
        },
      ],
    };
  },
  components: {
    PracticeCard,
  },
};
</script>
<style lang="scss" scoped>
.practice {
  padding: 50px 0px;
}
.practice-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
  text-align: center;
}
.practice-body-wrapper {
  display: flex;
  flex-direction: column;
  gap: 10px;
  .practice-wrapper__title {
    font-size: 35px;
    cursor: pointer;
    span {
      color: #22b111;
    }
  }
  .practice-wrapper__title:hover {
    text-decoration: underline;
  }
  .practice-wrapper__subtitle {
    color: rgba(17, 39, 52, 0.7);
    cursor: pointer;
  }
}
.practice-item-wrapper {
  display: flex;
  justify-content: center;
  gap: 25px;
}
.practice-card {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
  .practice-block-wrapper {
    padding: 7px 8px 3px 7px;
    background: rgba(241, 212, 75, 0.5);
    border-radius: 5px;
  }
  .practice-block-wrapper img {
    width: 70%;
    cursor: pointer;
  }
}
@media screen and (max-width: 992px) {
  .practice-card .practice-block-wrapper img {
    width: 70%;
  }
  .practice-card .practice-block-wrapper {
    padding: 2px 4px;
    border-radius: 4px;
  }
  .practice-body-wrapper .practice-wrapper__title {
    font-size: 30px;
  }
  .practice-body-wrapper .practice-wrapper__subtitle {
    font-size: 12px;
  }
}
@media screen and (max-width: 576px) {
  .practice-block-wrapper {
    display: none;
  }
  .practice-item-wrapper {
    flex-direction: column;
  }
}
</style>
