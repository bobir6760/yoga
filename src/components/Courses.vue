<template>
  <div class="courses">
    <div class="container">
      <div class="courses-wrapper">
        <div class="courses-wrapper-body">
          <div class="courses-wrapper__title">Courses</div>
          <div class="courses-wrapper__subtitle">
            Hone your skills with our professionally trained teachers who are
            passionate about yoga
          </div>
        </div>
        <div class="courses-wrapper-card">
          <CoursesCard
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
import CoursesCard from "@/components/CoursesCard";
export default {
  name: "Courses",
  data() {
    return {
      cards: [
        {
          title: "7 days of Relation",
          subtitle: "45 min",
        },
        {
          title: "Increase your mobility ",
          subtitle: "50 min",
        },
        {
          title: "Let`s begin some Yin",
          subtitle: "45 min",
        },
      ],
    };
  },
  components: {
    CoursesCard,
  },
};
</script>

<style lang="scss" scoped>
.courses {
  padding: 50px 0px;
}
.courses-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
}
.courses-wrapper-card {
  display: flex;
  gap: 30px;
  justify-content: center;
  flex-wrap: wrap;
}
.courses-wrapper-body {
  display: flex;
  flex-direction: column;
  gap: 10px;
  text-align: center;
  .courses-wrapper__title {
    font-size: 35px;
    cursor: pointer;
  }
}
.courses-wrapper__subtitle {
  cursor: pointer;
}
@media screen and (max-width: 992px) {
}
</style>
