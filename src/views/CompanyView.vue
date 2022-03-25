<template>
  <div class="company-c">
    <div class="company-hero">
      <div class="company-txt">
        <h1>Where designs are brought to life</h1>
        <h3>welcome to digitaL creation</h3>
      </div>
      <div>
        <div class="company-btn">
          <button class="btn-hero">
            <div class="btn-c">
              Get started <img src="../assets/arrow.svg" class="arrow" />
            </div>
          </button>
          <button class="btn-hide">
            <div class="btn-c">
              learn more <img src="../assets/arrow.svg" class="arrow hide" />
            </div>
          </button>
        </div>
      </div>
    </div>
  </div>
  <div class="img-c">
    <Img />
  </div>
  <div class="client-c">
    <Ourclients />
  </div>
  <div class="about-c">
    <About />
  </div>
  <div class="service-c">
    <Service />
  </div>
  <div class="portfolio-c">
    <Portfolio />
  </div>
  <div class="book-c">
    <Booking />
  </div>
  <div class="testimony-c">
    <Testimony />
  </div>
  <div class="contact-c">
    <Contact />
  </div>
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
<style>
@import "../style/companyView.css";
</style>
