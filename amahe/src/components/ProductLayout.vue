<script>
import star from "@/assets/etoile.png";
import ayurveda from "@/assets/ayurveda.png";
import swedish from "@/assets/swedish.png";
import shiatsu from "@/assets/shiatsu.png";
import bali from "@/assets/balinese.png";
import reflexo from "@/assets/reflexologie.png";
export default {
  data() {
      return {
        star: star,
        ayurveda: ayurveda,
        swedish: swedish,
        shiatsu: shiatsu,
        bali: bali,
        reflexo: reflexo,
        };
    },
}
</script>

<template>
  <div id="product">
    <h1 class="titles-components">
      Les massages que je vous propose
    </h1>
      <div class="container">
        <section class="massages">
          <!--Massage étoile-->
          <div class="massage-type">
            <div class="nav">
              <img class="icon" v-bind:src="star">
              <h3 class="massage-title">
                Massage étoile
              </h3>
            </div>
            <p>
              Appaisement et profonde relaxation par la stimulation des zones réflexes des cinq extrémités du corps (tête, mains, pieds)
            </p>
          </div>
          <!--Massage ayurvédique-->
          <div class="massage-type">
            <div class="nav">
              <img class="icon" v-bind:src="ayurveda">
              <h3 class="massage-title">
                Ayurvédique
              </h3>
            </div>
            <p>
              Relaxation profonde, permet de relâcher les tensions nerveuses et musculaires qui entravent la libre circulation de l'énergie dans le corps.ulation des zones réflexes des cinq extrémités du corps (tête, mains, pieds)
            </p>
          </div>
          <!--Massage suedois-->
          <div class="massage-type">
            <div class="nav">
              <img class="icon" v-bind:src="swedish">
              <h3 class="massage-title">
                Suédois
              </h3>
            </div>
            <p>
              Détend et relaxe le corps comme l’esprit. Particulièrement apaisant, il est apprécié pour sa capacité à diminuer les effets du stress sur le corps.            
            </p>
          </div>
          <!--Massage shiatsu-->
          <div class="massage-type">
            <div class="nav">
              <img class="icon" v-bind:src="shiatsu">
              <h3 class="massage-title">
                Shiatsu
              </h3>
            </div>
            <p>
              Étirements et pressions sur certains points de façon à faciliter la libre circulation de l'énergie.            
            </p>
          </div>
          <!--Massage balinais-->
          <div class="massage-type">
            <div class="nav">
              <img class="icon" v-bind:src="bali">
              <h3 class="massage-title">
                Balinais
              </h3>
            </div>
            <p>
              Harmonise différentes techniques à la fois relaxantes et énergétiques, douces et toniques. Il apporte ainsi une parfaite harmonie entre le corps et l’esprit.              
            </p>
          </div>
          <!--Massage réflexologie-->
          <div class="massage-type">
            <div class="nav">
              <img class="icon" v-bind:src="reflexo">
              <h3 class="massage-title">
                Réflexologie plantaire douce
              </h3>
            </div>
            <p>
              Relaxation profonde, bien-être global tant sur le plan physique que psychique et permet de relâcher les tensions.              
            </p>
          </div>
        </section>
      </div>
  </div>
</template>

<style scoped>
#product {
  margin-top: 2em;
}
.titles-components {
  color: #324B4E;
}
.massage-title,
p { 
  color: #548086;
}
.massage-title {
    font-weight: bold;
  }
  p {
    margin-top: 0.5em;
  }
/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  .titles-components {
  text-align: center;
  margin: 1em;
  padding-top: 1.5em;
}
  .massages {
    margin: 2em;
  }
  .massage-type {
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-radius: 1.5em;
    background-color: #eff8f0;
    padding: 1.5em;
    margin-bottom: 1.2em;
    height: 19em;
  }
  .nav {
    display: flex;
    align-items: center;
    margin-bottom: 0.5em;
  }
  .icon {
    width: 3em;
    margin-right: 0.9em;
  }
  
}
</style>