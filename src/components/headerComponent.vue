<template>
  <div class="header-c">
    <div class="nav">
      <div class="logo-container">
        <img src="../assets/logo.svg" alt="logo" class="logo" />
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
<style>
@import "@/style/header.css";
</style>
