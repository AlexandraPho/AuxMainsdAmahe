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
          "../src/assets/12.jpg",
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
            Je suis une masseuse expérimentée et attentionnée, dédiée à fournir des massages personnalisés pour aider mes clients à se détendre et à atteindre un état de bien-être. Je suis passionnée par mon métier et je m'efforce de m'améliorer constamment pour offrir une expérience de massage unique et sur mesure. Mon objectif est que mes clients se sentent apaisés, revitalisés et en paix après leur massage.
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
  .titles {
    color: #2f4858;
    font-family: 'Baskerville';
    font-style: italic;
  }
  /*Smartphone Size*/
  @media only screen and (max-width: 767px) {
  #aboutMe {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10em;
    background-color: #FFFAF1;
    margin: 1.6em;
    border-radius: 1em;
    padding: 2em;
  }
  .block-container {
    text-align: start;
    margin: 1.9em 1.5em;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
  }
  #aboutMe .portrait {
    width: 100%;
    height: auto;
  }
  .portrait {
   /* width: 23em;*/
    border-radius: 1em;
  }
  .text {
    color: #548086;
  }
  .titles {
    font-size: 2em;
    margin-bottom: 0.8em;
  }
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  #aboutMe {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10em;
    background-color: #FFFAF1;
    margin: 2.5em;
    padding: 3em;
    border-radius: 1em;
  }
  .block-container {
    text-align: start;
    margin: 1.9em 1.5em;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    padding: 1.5em;
  }
  #aboutMe .portrait {
    width: 35em;
    height: auto;
  }
  .portrait {
    border-radius: 1em;
  }
  .text {
    color: #548086;
  }
  .titles {
    font-size: 2.8em;
    margin-bottom: 0.8em;
  }
  p {
    font-size: 1.2em;
  }
}

/* Large devices (large laptops and desktops, 992px and up) */
@media only screen and (min-width: 992px) {
  #aboutMe {
    margin-top: 10em;
    display: flex;
    justify-content: center;
    background-color: #FFFAF1;
    border-radius: 1.5em;
    padding: 2.5em;

  }
  #aboutMe .portrait {
    display: flex;
    width: 35em;
    margin: 1em;
    border-radius: 1.5em;
    height: auto;
  }
  .block-container {
    padding: 2em;
    width: 60em;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .titles {
    margin-bottom: 0.5em;
  }
  .text {
    width: 80%;
    text-align: center;
  }
  p {
    font-size: 1.2em;
    margin-top: 1em;
  }
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  #aboutMe {
    margin-top: 10em;
    display: flex;
    justify-content: center;
    flex-direction: row-reverse;
    background-color: #FFFAF1;
    border-radius: 1.5em;
    padding: 2.5em;

  }
  #aboutMe .portrait {
    display: flex;
    width: 30em;
    margin: 1em;
    border-radius: 1.5em;
    height: auto;
  }
  .block-container {
    padding: 2em;
    width: 60em;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  .titles {
    margin-bottom: 0.5em;
  }
  .text {
    width: 80%;
    text-align: start;
  }
  p {
    font-size: 1.2em;
    margin-top: 1em;
  }
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  #aboutMe {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 10em;
    background-color: #FFFAF1;
    margin: 2.5em;
    padding: 3em;
    border-radius: 1em;
  }
  .block-container {
    text-align: start;
    margin: 1.9em 1.5em;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    padding: 1.5em;
  }
  #aboutMe .portrait {
    width: 35em;
    height: auto;
  }
  .portrait {
    border-radius: 1em;
  }
  .text {
    color: #548086;
  }
  .titles {
    font-size: 2.8em;
    margin-bottom: 0.8em;
  }
  p {
    font-size: 1.2em;
  }
}

/* Large devices (large laptops and desktops, 992px and up) */
@media only screen and (min-width: 992px) {
  #aboutMe {
    margin-top: 10em;
    display: flex;
    justify-content: center;
    background-color: #FFFAF1;
    border-radius: 1.5em;
    padding: 2.5em;

  }
  #aboutMe .portrait {
    display: flex;
    width: 35em;
    margin: 1em;
    border-radius: 1.5em;
    height: auto;
  }
  .block-container {
    padding: 2em;
    width: 60em;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .titles {
    margin-bottom: 0.5em;
  }
  .text {
    width: 80%;
    text-align: center;
  }
  p {
    font-size: 1.2em;
    margin-top: 1em;
  }
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  #aboutMe {
    margin-top: 10em;
    display: flex;
    justify-content: center;
    flex-direction: row-reverse;
    background-color: #FFFAF1;
    border-radius: 1.5em;
    padding: 2.5em;

  }
  #aboutMe .portrait {
    display: flex;
    width: 30em;
    margin: 1em;
    border-radius: 1.5em;
    height: auto;
  }
  .block-container {
    padding: 2em;
    width: 60em;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  .titles {
    margin-bottom: 0.5em;
  }
  .text {
    width: 80%;
    text-align: start;
  }
  p {
    font-size: 1.2em;
    margin-top: 1em;
  }
}
</style>
