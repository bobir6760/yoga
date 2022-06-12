<template>
  <div class="member">
    <div class="container">
      <div class="member-wrapper">
        <div class="member-wrapper-card">
          <div class="member-wrapper__title">
            Member <span> Benefits </span>
          </div>
        </div>
        <div class="member-wrapper-card">
          <MemberCard
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
import MemberCard from "@/components/MemberCard";
export default {
  name: "Member",
  data() {
    return {
      cards: [
        {
          title: "World Class Teacher",
          subtitle:
            "Experience the depth of knowledge from experts across all areas of yoga.",
          imgUrl: require("@/assets/img/IMG1.png"),
        },
        {
          title: "Stay Inspired",
          subtitle:
            "Explore hundreds of live & on-demand classes, with new content added daily.",
          imgUrl: require("@/assets/img/IMG2.png"),
        },
        {
          title: "Everywhere You Are",
          subtitle:
            "Take classes at your own pace, on your own time, and on any device.",
          imgUrl: require("@/assets/img/IMG3.png"),
        },
      ],
    };
  },
  components: {
    MemberCard,
  },
};
</script>

<style lang="scss" scoped>
.member {
  padding: 50px 0px;
}
.member-wrapper {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 50px;
}
.member-wrapper__title {
  font-size: 35px;
  cursor: pointer;
  span {
    color: #22b111;
  }
}
.member-wrapper__title:hover {
  text-decoration: underline;
}
.member-wrapper-card {
  display: flex;
  justify-content: center;
  gap: 20px;
}
@media screen and (max-width: 992px) {
  .member-wrapper-card {
    display: flex;
    justify-content: center;
    gap: 20px;
  }
}
@media screen and (max-width: 576px) {
  .member-wrapper-item {
    display: flex;
    flex-direction: column;
  }
  .member-wrapper-card {
    display: flex;
    justify-content: center;
    flex-direction: column;
    gap: 20px;
  }
}
</style>
