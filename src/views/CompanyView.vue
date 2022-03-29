<template>
  <div class="company">
    <div class="company-hero" ref="hero">
      <div class="company-txt">
        <h1>Where designs are brought to life</h1>
        <h3>welcome to digitaL creation</h3>
      </div>
      <div>
        <div class="company-btn">
          <button class="btn-hero">
            <div class="btn-c">
              Get started
              <img src="../assets/arrow.svg" class="arrow" @click="start()" />
            </div>
          </button>
          <button class="btn-hide">
            <div class="btn-c">
              learn more
              <img
                src="../assets/arrow.svg"
                class="arrow hide"
                @click="learn()"
              />
            </div>
          </button>
        </div>
      </div>
    </div>
  </div>
  <div class="img-container">
    <Img />
  </div>
  <div class="constrain">
    <Ourclients />
    <About />
    <Service />
    <Portfolio />
    <Booking class="book-with-us" />
    <Testimony />
  </div>
  <Contact ref="contact" />
</template>
<script setup>
import About from "../views/AboutView.vue";
import Img from "../components/imgCompany.vue";
import Service from "../views/ServiceView.vue";
import Contact from "../views/ContactView.vue";
import Ourclients from "../components/ourClients.vue";
import Booking from "../components/bookingComponent.vue";
import Testimony from "../components/testimonyComponent.vue";
import Portfolio from "../components/portfolioComponent.vue";
</script>
<script>
import gsap from "gsap";
export default {
  data() {
    return {};
  },

  mounted() {
    const { hero } = this.$refs;
    const tl = gsap.timeline({});
    tl.from(hero, {
      duration: 3,
      x: -700,
      ease: "power3.out",
    });
  },

  methods: {
    start() {
      this.$router.push({ name: "service" });
    },
    learn() {
      this.$router.push({ name: "about" });
    },
  },
};
</script>

<style>
@import "../style/companyView.css";
</style>
