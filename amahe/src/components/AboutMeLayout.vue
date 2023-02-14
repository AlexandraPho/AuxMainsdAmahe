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
            Bienvenue à tous!
          </h2>
          <p>
            Je suis heureuse de vous présenter mon métier de masseuse, où je fais en sorte que chaque massage soit un moment de détente et de bien-être, sans compterque c'est avant tout une passion pour moi.
            En tant que masseuse, j'ai la chance d'avoir un lien privilégié avec mes clients et de pouvoir les aider à atteindre un bien-être grâce à mon toucher. Je suis une personne à l’écoute et hypersensible, et ces qualités se reflètent dans mon approche personnalisée et bienveillante du massage. 
            Je suis toujours en train de me former pour vous offrir une expérience unique et sur mesure. Mon objectif est de vous offrir un moment de détente, de soulager votre stress et votre anxiété, et de vous aider à vous sentir en paix, apaisé et revitalisé.
            Je suis convaincue que le massage peut avoir un impact profond sur le corps et l'esprit, et c'est pour cette raison que je m'efforce d'apporter une touche de douceur et de bonté à chaque massage. Je veux que mes clients se sentent entendus et pris en charge, et je m'engage à être à l'écoute de leurs besoins et de leurs souhaits.
            Mon objectif est que vous vous sentiez apaisés, revitalisés et en paix lorsque vous quittez ma table de massage.
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