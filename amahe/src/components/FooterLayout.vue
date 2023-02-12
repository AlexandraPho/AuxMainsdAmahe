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
              <span class="title-footer">Aux mains d'Amahé</span>

          </div>
          </a>
        </div>
        <div class="social-media">
          <a class="icon" href="https://www.facebook.com/auxmainsdamahe" target="_blank"><img class="fb-icon" alt="facebook-logo" v-bind:src="fb"></a>
          <a class="icon" href="https://www.instagram.com/aux_mains_damahe/" target="_blank"><img class="inst-icon" alt="instagram-logo" v-bind:src="inst"></a>
        </div>
        <div class="condition">
          <a href="#" class="condition-footer">Code Déontologique</a>
          <p class="condition-footer">|</p>
          <a href="#" class="condition-footer">CGV</a>
        </div>
        <div class="createBy">
          <p>
            Copyright All Right Reserved 2023 - Alexandra Pinheiro
          </p>
        </div>
    </section>
  </footer>
</template>

<style scoped>
#footer {
  height: 18em;
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
    display: flex;
    flex-direction: column;
    justify-content: space-around;
  }
  .link-header {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .social-media {
    display: flex;
    justify-content: space-evenly;
    margin-bottom: 1.2em;
  }
  .logo {
    width: 8em;
  }
  .title-footer {
    font-weight: 500;
  }
  .fb-icon {
    width: 1.9em;
  }
  .condition {
    display: flex;
    justify-content: center;
  }
  .condition-footer {
    margin: 0.5em;
  }
  .createBy {
    font-size: x-small;
  }
}
</style>