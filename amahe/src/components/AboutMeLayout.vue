<script>
import portrait from "@/assets/portrait.png";

export default {
  data() {
      return {
        portrait: portrait,
        };
    },
}
</script>

<template>
  <div id="aboutMe">
    <img class="portrait" v-bind:src="portrait">
      <section class="block-container">
        <div class="text">
          <h3 class="titles">
            À l'écoute de votre corps
          </h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec eu massa a turpis commodo fermentum. Ut euismod leo et lacinia mattis. Integer quis risus quam. Donec dui libero, sollicitudin ultricies mattis eu, tincidunt bibendum sapien. Sed iaculis, ex quis pellentesque luctus, massa dolor ultricies mauris, a feugiat est quam at nisi. In mollis, mi eu tincidunt cursus, ligula massa rhoncus odio, sed auctor velit tortor at quam.
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
  
  .portrait {
    max-width: 100%;
  }
}
</style>