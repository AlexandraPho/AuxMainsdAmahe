<script>
import hand1 from "@/assets/hand1.jpg";

export default {
  data() {
      return {
        hand1: hand1,
        };
    },
}
</script>

<template>
  <div id="main">
    <img class="hand1" v-bind:src="hand1">
      <section class="block-container">
        <div class="text">
          <h2 class="first-title"> 
            <span class="first-span-title">Aux mains d'</span>
            <span class="second-span-title">Amahé</span>
          </h2>
          <!--<h3 class="second-title">
            À l'écoute de votre corps
          </h3>-->
          <p>
            Si vous êtes à la recherche d'un moment de détente, de mieux-être, ou si vous voulez simplement prendre soin de vous, je serais ravie de vous rencontrer et de vous aider à atteindre votre bien-être optimal.          
          </p>
        </div>
        <button class="btn-form"><a href="#product" class="button">Les massages</a></button>
      </section>
  </div>
</template>

<style scoped>
  #main {
    display: flex;
    align-items: center;
  }
  .hand1 {
    max-width: 100%;
    margin-top: 9em;
    filter: brightness(0.6);
  }

  .first-span-title {
    font-weight: bold;
  }
  .second-span-title {
    font-family: 'Baskerville';
    margin-left: 0.3em;
    font-style: italic;
    font-weight: 500;
  }
  .btn-form {
    border: none;
    display: block;
    text-align: center;
    cursor: pointer;
    outline: none;
    overflow: hidden;
    position: sticky;
    font-weight: 500;
    box-shadow: 0 5px 15px rgba(0,0,0,0.20);
    background-color: #eff8f0;
    padding: 0.9em;
    border-radius: 2em;
  }
  a {
    text-decoration: none;
  }
  .btn-form a {
    font-weight: bold;
    position: relative; 
    z-index: 1;
    color: #2f4858;
  }
  .btn-form:after {
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    height: 350%;
    width: 190%;
    background: #89b68e;
    -webkit-transition: all .5s ease-in-out;
    transition: all .5s ease-in-out;
    -webkit-transform: translateX(-98%) translateY(-25%) rotate(45deg);
    transform: translateX(-98%) translateY(-25%) rotate(45deg);
  }
  .btn-form:hover:after {
    -webkit-transform: translateX(-9%) translateY(-25%) rotate(45deg);
    transform: translateX(-9%) translateY(-25%) rotate(45deg);
  }
  a:hover {
    color: black;
  }
  p {
    color: #548086;
  }

  /*Smartphone Size*/
  /* Extra small devices (phones, 439px and down) */
  @media only screen and (max-width: 439px) {
  #main {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 1.5em;
  }
  .block-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1.4em;
  }
  .office {
    display: none;
  }
  .hand1 {
    margin-top: 6em;
    max-width: 100%;
  }
  .first-title {
    position: absolute;
    top: 17.5%;
    left: 45%;
    transform: translate(-40%, 55%);
  }
  .first-span-title,
  .second-span-title {
    color: white;
    font-size: 1.3em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
  .span-title {
    font-family: fantasy;
    margin-left: 0.3em;
    font-style: italic;
    font-size: 1.1em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
}

/* Small devices (portrait tablets and large phones, 440px and up) */
  @media (min-width: 440px){
  #main {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 1.5em;
  }
  .block-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1.5em;
  }
  .office {
    display: none;
  }
  .hand1 {
    margin-top: 7em;
    max-width: 100%;
  }
  .first-title {
    position: absolute;
    top: 18%;
    left: 45%;
    transform: translate(-40%, 60%);
  }
  .first-span-title,
  .second-span-title {
    color: white;
    font-size: 1.8em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
  .span-title {
    font-family: fantasy;
    margin-left: 0.3em;
    font-style: italic;
    font-size: 1.1em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
}

/* Small devices (portrait tablets and large phones, 520px and up) */
@media (min-width: 520px){
  #main {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 1.5em;
  }
  .block-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1.5em;
  }
  .office {
    display: none;
  }
  .hand1 {
    margin-top: 7em;
    max-width: 100%;
  }
  .first-title {
    position: absolute;
    top: 20%;
    left: 45%;
    transform: translate(-40%, 60%);
  }
  .first-span-title,
  .second-span-title {
    color: white;
    font-size: 2em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
  .span-title {
    font-family: fantasy;
    margin-left: 0.3em;
    font-style: italic;
    font-size: 1.1em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  #main {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 2em;
  }
  .block-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1.5em;
  }
  .office {
    display: none;
  }
  .hand1 {
    margin-top: 8em;
    max-width: 100%;
  }
  .first-title {
    position: absolute;
    top: 24%;
    left: 45%;
    transform: translate(-40%, 60%);
  }
  .first-span-title,
  .second-span-title {
    color: white;
    font-size: 2.5em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
  .span-title {
    font-family: fantasy;
    margin-left: 0.3em;
    font-style: italic;
    font-size: 1.1em;
  }
  p,
  .btn-form {
    font-size: 1.2em;
  }
  .btn-form {
    margin-top: 1.2em;
  }
}


/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
  #main {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 2em;
  }
  .block-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1.5em;
  }
  .office {
    display: none;
  }
  .hand1 {
    margin-top: 8em;
    max-width: 100%;
  }
  .first-title {
    width: 15em;
    position: absolute;
    top: 28%;
    left: 45%;
    transform: translate(-40%, 60%);
  }
  .first-span-title,
  .second-span-title {
    color: white;
    font-size: 2.5em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
  .span-title {
    font-family: fantasy;
    margin-left: 0.3em;
    font-style: italic;
    font-size: 1.1em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
}
/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  #main {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 2em;
  }
  .block-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1.5em;
  }
  .office {
    display: none;
  }
  .hand1 {
    margin-top: 8em;
    max-width: 100%;
  }
  .first-title {
    width: 16em;
    position: absolute;
    top: 30%;
    left: 45%;
    transform: translate(-40%, 60%);
  }
  .first-span-title,
  .second-span-title {
    color: white;
    font-size: 2.5em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
  .span-title {
    font-family: fantasy;
    margin-left: 0.3em;
    font-style: italic;
    font-size: 1.1em;
  }
  .text {
    text-align: center;
    margin-bottom: 1.8em;
  }
}
</style>