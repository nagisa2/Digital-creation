<template>
  <div class="booking">
    <div class="booking-cfg">
      <div class="booking-info">
        <div class="card-info">
          <h1>Wanna get started right away, call us</h1>
          <p>
            Call us and tell us what u want so we can get started with your
            designs
          </p>
          <div class="call-span">
            <div class="call-cfg">
              <img src="../assets/call.svg" alt="call" class="phone-icon" />
              <span>0722925034</span>
            </div>
          </div>
        </div>
      </div>
      <div class="booking-card">
        <div class="b-card">
          <div class="book-title">
            <h1>Book with us</h1>
          </div>
          <form class="booking-form" @submit.prevent="Book()">
            <input
              type="text"
              v-model="form.Name"
              placeholder="Name"
              class="booking-input"
              required
            />
            <input
              type="text"
              v-model="Phone"
              placeholder="Phone number"
              class="booking-input"
            />
            <textarea
              v-model="form.Message"
              placeholder="Tell us what you want"
              class="booking-textarea"
              required
            />
            <button class="booking-btn" type="submit">Book now</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      form: {
        Name: "",
        Phone: "",
        Message: "",
      },
    };
  },

  methods: {
    Book() {
      let { Name, Message } = this.form;
      location.href = `https://wa.me/254722925034/?text=Hi, iam ${Name}, ${Message}`;
    },
  },
};
</script>
<style>
@import "../style/booking.css";
</style>
