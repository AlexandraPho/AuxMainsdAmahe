<script>
  import CarouselItem from "../components/CarouselItem.vue"
  import CarouselControls from "../components/CarouselControls.vue"

  export default {
    props: ['slides'],
    components: {
      CarouselItem,
      CarouselControls,
    },
    data: () => ({
      currentSlide: 0,
      slideInterval: null,
      direction: "right" 
    }),
    methods: {
      setCurrentSlide(index) {
        this.currentSlide = index;
      },
      prev() {
        const index = 
          this.currentSlide > 0 ? this.currentSlide - 1 : this.slides.lenght - 1;
          this.setCurrentSlide(index);
          this.direction = "left";
          this.startSlideTimer();
      },
      _next() {
        const index = 
          this.currentSlide < this.slides.length -1 ? this.currentSlide + 1 : 0;
          this.setCurrentSlide(index);
          this.direction = "right";
      },
      next() {
        this._next();
          this.startSlideTimer();
      },
      startSlideTimer() {
        //this.slideInterval = setInterval(() => {
         // this._next();
        //}, 3000);
      },
      stopSlideTimer() {
        clearInterval(this.slideInterval);
      },
    },
    mounted () {
      this.startSlideTimer();
    },
    beforeUnmount () {
      this.stopSlideTimer();
    }
  }
</script>


<template>
  <div class="carousel">
    <div class="carousel-inner">
      <carousel-item 
        v-for="(slide, index) in slides" 
        :slide="slide" 
        :key="`item-${index}`"
        :current-slide="currentSlide"
        :index="index"
        :direction="direction"
      ></carousel-item>
      <carousel-controls @prev="prev" @next="next"></carousel-controls>
    </div>
  </div>
</template>

<style scoped>
 .carousel {
  display: flex;
  justify-content: center;
 }
 .carousel-inner {
  position: relative;
  width: 280px;
  height: 225px;
  overflow:hidden;
  border-radius: 1em;
    margin-top: 1.8em;
 }
</style>