<template>
  <div class="container">
    <h1>Home Page</h1>
    <div class="box" ref="box">Home</div>
    <p>
      <nuxt-link to="/about">About Page</nuxt-link>
    </p>
  </div>
</template>

<script>
// Notice how gsap is being transpiled in nuxt.config.js
import { gsap } from "gsap";

export default {
  mounted() {
    gsap.to(this.$refs.box, { rotation: "+=360" });
  },
};
</script>

<style scoped></style>
