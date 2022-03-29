<template>
  <div class="header">
    <div class="nav" ref="nav">
      <div class="logo-container">
       <a href="/"><img src="../assets/logo.svg" alt="logo" class="logo" /></a>
      </div>
      <div class="nav-links">
        <RouterLink to="/" class="link">Company</RouterLink>
        <RouterLink to="/about" class="link">About</RouterLink>
        <RouterLink to="/service" class="link">Service</RouterLink>
        <RouterLink to="/contact" class="link">Contact</RouterLink>
      </div>
    </div>
  </div>
  <RouterView />
</template>
<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>
<script>
import gsap from "gsap";
export default {
  data() {
    return {};
  },

  mounted() {
    const { nav } = this.$refs;
    const tl = gsap.timeline({});
    tl.from(nav, {
      duration: 2.5,
      y: -200,
      ease: "power3.out",
    });
  },
};
</script>

<style>
@import "@/style/header.css";
</style>
