<script>
import office2 from "@/assets/office-2.jpg";
import hand1 from "@/assets/hand1.jpg";

export default {
  data() {
      return {
        office2: office2,
        hand1: hand1,
        };
    },
}
</script>

<template>
  <div id="main">
    <div class="home">
      <h2 class="first-title"> 
        <span class="first">Aux mains </span><br>
        <span class="second">d'Amahé</span>
      </h2>
      <img class="hand1" v-bind:src="hand1">
    </div>
    <img class="office" v-bind:src="office2">
      <section class="block-container">
        <div class="text">
          <h3 class="second-title">
            À l'écoute de votre corps
          </h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec eu massa a turpis commodo fermentum. 
          </p>
        </div>
      </section>
  </div>
</template>

<style scoped>

  #main {
    display: flex;
    align-items: center;
  }


  /*Smartphone Size*/
  @media only screen and (max-width: 680px) {
  #main {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 1.5em;
  }
  .home {
    background-image: url;
  }
  .hand1 {
    margin-top: 8em;
    width: 100%;
    height: 35em;
    object-fit: cover;
    /* display: block; */
    margin-right: auto;
    margin-left: auto;
    clip-path: polygon(0% 0%,100% 0%,100% 100%,0% 100%);
  }
  .first-title {
    position: absolute;
    top: 45%;
    left: 45%;
    transform: translate(-40%, 60%);
  }
  .first {
    color: white;
    font-weight: 600;
    font-size: 1.5em;
  }
  .second {
    color: white;
    font-style: italic;
    font-family: fantasy;
    margin-left: 1.4em;
    font-size: 1.5em;
  }
  .office {
    max-width: 100%;
  }
}
</style>