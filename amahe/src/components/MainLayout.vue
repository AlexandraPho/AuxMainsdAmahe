<script>
import office from "@/assets/office.jpeg";

export default {
  data() {
      return {
        office: office,
        };
    },
}
</script>

<template>
  <div id="main">
    <img class="office" v-bind:src="office"> 
    <!--<h2 class="titles-components">
      A propos de moi
    </h2>-->
      <section class="block-container">
        <div class="text">
          <h2 class="first-title"> 
            <span>Aux mains d'</span><br>
            <span>Amahé</span>
          </h2>
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
  
  .office {
    margin-top: 8em;
    max-width: 100%;
  }
}
</style>