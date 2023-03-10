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
            <span class="title-footer">Aux mains d'</span>
            <span class="second-title-footer">Amahé</span>
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
  display: flex;
  justify-content: center;
  background-color: #FFFAF1;
}
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
.condition {
  display: flex;
  justify-content: center;
  margin-bottom: 0.5em;
}
a {
  text-decoration: none;
  color: #2F4858;
}
p {
  color: #548086;
}
.second-title-footer {
  font-family: 'baskerville';
  font-style: italic;
}

/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  #footer {
    height: 18em;
  }
  .logo {
    width: 8em;
  }
  .title-footer {
    font-weight: 500;
  }
  .second-title-footer {
  font-size: 1.2em;
  }
  .fb-icon {
    width: 1.9em;
  }
  .condition-footer {
    margin: 0.5em;
  }
  .createBy {
    font-size: x-small;
  }
}

/* Medium devices (landscape tablets, 681px and up) */
@media only screen and (min-width: 681px) {
  #footer {
    height: 25em;
  }
  .logo {
    width: 15em;
  }
  .title-footer {
    font-weight: 500;
    font-size: x-large;
  }

  .fb-i.second-title-footer {
  font-size: 1.2em;
  }con,
  .inst-icon {
    width: 3em;
  }
  .condition-footer {
    margin: 0.5em;
    font-size: large;
  }
  .createBy {
    font-size: normal;
    margin-bottom: 1em;
  }
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  #footer {
    height: 25em;
  }
  .logo {
    width: 15em;
  }
  .title-footer {
    font-weight: 500;
    font-size: x-large;
  }
  .second-title-footer {
  font-size: 1.8em;
  }
  .fb-icon,
  .inst-icon {
    width: 3em;
  }
  .condition-footer {
    margin: 0.5em;
    font-size: large;
  }
  .createBy {
    font-size: normal;
    margin-bottom: 1em;
  }
}


/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  #footer {
    height: 25em;
  }
  .logo {
    width: 15em;
  }
  .title-footer {
    font-weight: 500;
    font-size: x-large;
  }
  .fb-icon,
  .inst-icon {
    width: 3em;
    margin: 1em;
  }
  .condition {
    display: flex;
    justify-content: center;
  }
  .createBy {
    font-size: normal;
    margin-bottom: 1em;
  }
}
</style>