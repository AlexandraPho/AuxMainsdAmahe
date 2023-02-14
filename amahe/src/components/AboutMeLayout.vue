<script>
import portrait from "@/assets/portrait.png";
import Carousel from "../components/carousel/Carousel.vue";

export default {
  components : {
    Carousel
  },
  data() {
      return {
        portrait: portrait,
        slides: [
          "src/assets/12.jpg",
          "src/assets/13.jpg",
          "src/assets/hand2.jpg",
          "src/assets/hand5.jpg",
          "src/assets/amahe2.jpg",
        ],
        
      }
    },
    
  components : {
    Carousel,
  },
}
</script>

<template>
  <div id="aboutMe">
    <img class="portrait" v-bind:src="portrait">
      <section class="block-container">
        <div class="text">
          <h2 class="titles">
            À propose de moi
          </h2>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec eu massa a turpis commodo fermentum. Ut euismod leo et lacinia mattis. Integer quis risus quam. Donec dui libero, sollicitudin ultricies mattis eu, tincidunt bibendum sapien. Sed iaculis, ex quis pellentesque luctus, massa dolor ultricies mauris, a feugiat est quam at nisi. In mollis, mi eu tincidunt cursus, ligula massa rhoncus odio, sed auctor velit tortor at quam.
          </p>
        </div>
        <carousel :slides="slides" :interval="4000" controls indicators></carousel>
      </section>
  </div>
</template>

<style scoped>
  #main {
    display: flex;
    align-items: center;
  }
  #aboutMe .portrait {
    width: 100%;
    height: auto;
  }
  /*Smartphone Size*/
  @media only screen and (max-width: 680px) {
  #aboutMe {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10em;
    background-color: #F8F1E3;
    margin: 1.6em;
    border-radius: 1em;
  }
  .block-container {
    text-align: start;
    margin: 1.9em 1.5em;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .portrait {
   /* width: 23em;*/
    border-radius: 1em;
  }
  .text {
    color: #548086;
  }
  .titles {
    font-size: x-large;
    font-weight: 600;
    margin-bottom: 0.8em;
  }
  
}
</style>