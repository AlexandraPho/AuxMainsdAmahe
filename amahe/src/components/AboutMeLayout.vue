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
          <h2 class="titles">
            À propose de moi
          </h2>
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
  }
  .portrait {
    width: 23em;
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