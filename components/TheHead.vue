<template>
  <main>
    <section class="flex-container">
      <div class="title-container">
        <h1>Álvaro Belmonte</h1>
        <h2>
          Hi, I'm a
          <b>web developer</b> based in Alicante (Spain)
        </h2>
      </div>
      <div class="animation-container">
        <lottie
          class="confetti-container"
          :width="lottieWidth"
          :height="lottieHeight"
          :options="lottieOptions"
          v-on:animCreated="handleAnimation"
        />
      </div>
    </section>
  </main>
</template>

<script>
import Lottie from "vue-lottie";
import * as animationData from "~/static/lottie/programming.json";

export default {
  components: {
    Lottie,
  },
  data() {
    return {
      anim: null,
      lottieOptions: { animationData: animationData.default, loop: true },
    };
  },
  methods: {
    handleAnimation: function (anim) {
      this.anim = anim;
    },
  },
  computed: {
    lottieHeight() {
      return window.innerHeight / 2;
    },
    lottieWidth() {
      return window.innerWidth / 3;
    },
  },
};
</script>

<style >
main {
  min-height: 60vh;
}
h1 {
  color: #fa4b38;
  font-size: 2rem;
  text-align: center;
  font-family: "Heebo", sans-serif;
  padding-top: 2rem;
}

h2,
h3,
h4 {
  font-family: "Spartan", sans-serif;
}
h2 {
  padding: 0;
  font-size: 1rem;
  margin: 0;
}

.flex-container {
  padding: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.title-container {
  margin-right: 5%;
}
.animation-container {
  background-color: transparent;
}

@media only screen and (min-width: 720px) {
  h1 {
    font-size: 4rem;
    text-align: left;
    padding-top: 0;
  }
}
</style>