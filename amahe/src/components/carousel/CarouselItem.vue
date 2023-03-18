<script>
export default {
  emits: ["mouseenter", "mouseout"],
  props: ["slide", "currentSlide", "index", "direction"],
  computed: {
    transitionEffect() {
      return this.direction === "right" ? "slide-out" : "slide-in";
    },
  },
};
</script>

<template>
  <transition :name="transitionEffect">
    <div
      class="carousel-item"
      v-show="currentSlide === index"
      @mouseenter="$emit('mouseenter')"
      @mouseout="$emit('mouseout')"
    >
     
      <img :src="slide.img" alt="loading">
    </div>
  </transition>
</template>

<style scoped>

img {
  width : 300px;
  height : auto;
  }
.carousel-item {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}
.slide-in-enter-active,
.slide-in-leave-active,
.slide-out-enter-active,
.slide-out-leave-active {
  transition: all 1s ease-in-out;
}
.slide-in-enter-from {
  transform: translateX(-100%);
}
.slide-in-leave-to {
  transform: translateX(100%);
}
.slide-out-enter-from {
  transform: translateX(100%);
}
.slide-out-leave-to {
  transform: translateX(-100%);
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  img {
    width: 450px;
  }
}

/* Medium devices (landscape tablets, 1200px and up) */
@media only screen and (min-width: 1200px) {
  img {
    width: 400px;
  }
}
</style>
