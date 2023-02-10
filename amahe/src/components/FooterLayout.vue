<script>
import logo from "@/assets/fleur.svg";

export default {
  data() {
      return {
        logo: logo,
        };
    },
};
</script>

<template>
  <footer id="footer">
    <section class="">
        <div class="logo-container">
          <!--LOGO-->
          <a href ="#main" class="link-header">
          <img class="logo" v-bind:src="logo">
          <div class="text-container">
              <span class="first-part">Aux mains </span>
              <span class="second-part">d'Amahé</span>
          </div>
        </a>
        </div>
    </section>
  </footer>
</template>

<style scoped>

</style>