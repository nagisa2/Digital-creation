<template>
  <div class="contact">
    <div class="contact-container">
      <div class="contact-heading">
        <div class="contact-info-h">
          <h1>Are you instrested in working with us?</h1>
        </div>
        <div class="contact-btn">
          <button class="btn-heading" @click="whatsapp()">
            <div class="btn-cfg">
              Let's chat <img src="../assets/arrow-green.svg" class="arrow-h" />
            </div>
          </button>
          <button class="btn-hide-h">
            <div class="btn-cfg">
              Book now
              <img src="../assets/arrow-green.svg" class="arrow hide" />
            </div>
          </button>
        </div>
      </div>
      <hr class="line" />
      <div class="contacts-link-container">
        <div class="contacts-link-a">
          <h1>Contact information</h1>
          <h3>get in touch with us if u need any help</h3>
          <div class="contact-links">
            <div class="contact-link">
              <img src="../assets/call.svg" class="contact-icon" /><span
                >0722925034</span
              >
            </div>
            <div class="contact-link">
              <img src="../assets/email.svg" class="contact-icon" /><span
                >design@digitalcreation.gmail.com</span
              >
            </div>
            <div class="contact-link">
              <img src="../assets/location.svg" class="contact-icon" />
              <div class="location">
                <span>Nairobi,Munyu road</span>
                <span>Munyu business center, Floor4,E3</span>
              </div>
            </div>
          </div>
        </div>
        <div class="contacts-link-b">
          <h1>Our social platform</h1>
          <h3>check out our social media platforms</h3>
          <div class="social-container">
            <div class="social-link">
              <img
                src="../assets/whatsapp.svg"
                alt="whatsapp"
                class="social-icon"
                @click="whatsapp()"
              />
              <img
                src="../assets/Instagram.svg"
                alt="instagram"
                class="social-icon"
              />
              <img
                src="../assets/Twitter.svg"
                alt="twitter"
                class="social-icon"
              />
              <img
                src="../assets/Facebook.svg"
                alt="facebook"
                class="social-icon"
              />
            </div>
            <div class="footer">
              <h1>&#169;Digital creation@2022</h1>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },

  methods: {
    facebook() {},

    whatsapp() {
      window.open(
        "https://web.whatsapp.com/send?text==Hi, i wanna know more about your design work &phone=0722925034",
        "Share with Whatsapp Web",
        "width=800,height=600"
      );
    },
  },
};
</script>
<style>
@import "../style/contactView.css";
</style>
