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
    <!--<img class="office" v-bind:src="office">-->
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
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec eu massa a turpis commodo fermentum. 
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
  }
  .btn-form {
    border: none;
    display: block;
    text-align: center;
    cursor: pointer;
    outline: none;
    overflow: hidden;
    position: relative;
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
  @media only screen and (max-width: 680px) {
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
  .hand1 {
    margin-top: 9em;
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
    font-weight: 600;
    font-size: 1.5em;
  }
  .second-span-title {
    font-family: fantasy;
    margin-left: 0.3em;
    font-style: italic;
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