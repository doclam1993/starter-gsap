<template>
  <div class="container">
    <h1>About Page</h1>
    <div class="box" ref="box">About</div>
    <p>
      <nuxt-link to="/">Back home</nuxt-link>
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
