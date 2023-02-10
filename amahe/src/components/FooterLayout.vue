<script>
import logo from "@/assets/logoFooter.svg";
import fb from "@/assets/fb.png";
import inst from "@/assets/inst.png";

export default {
  data() {
      return {
        logo: logo,
        fb: fb,
        inst:inst
        };
    },
};
</script>

<template>
  <footer id="footer">
    <section class="footer-container">
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
        <div class="social-media">
          <img class="fb-icon" v-bind:src="fb">
          <img class="inst-icon" v-bind:src="inst">
        </div>
        <div class="condition">

        </div>
    </section>
  </footer>
</template>

<style scoped>
#footer {
  height: 15em;
  display: flex;
  justify-content: center;
  background-color: #FFFAF1;
}
a {
  text-decoration: none;
  color: #2F4858;
}

/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  .footer-container {
   
  }
  .social-media {
    display: flex;
    justify-content: center;
    align-items: flex-end;
  }
  .logo {
    width: 10em;
  }
  .fb-icon {
    width: 1.9em;
  }
}
</style>