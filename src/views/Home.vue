<template>
  <div class="home">
    <Navbar />
    <Best />
    <Member />
    <Time />
    <Challenge />
    <Courses />
    <Practice />
    <From />
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Best from "@/components/Best.vue";
import Member from "@/components/Member.vue";
import Time from "@/components/Time.vue";
import Challenge from "@/components/Challenge.vue";
import Courses from "@/components/Courses.vue";
import Practice from "@/components/Practice.vue";
import From from "@/components/From.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    Best,
    Member,
    Time,
    Challenge,
    Courses,
    Practice,
    From,
    Footer,
  },
};
</script>
