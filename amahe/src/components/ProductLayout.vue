<script>
import contact from "@/assets/phoneMail.png";
import adress from "@/assets/adress.png";
import calendar from "@/assets/calendar.png";
import phone from "@/assets/phone.png";
import mail from "@/assets/mail.png";

export default {
  data() {
      return {
        contact: contact,
        phone: phone,
        mail: mail,
        adress: adress,
        calendar: calendar
        };
    },
}
</script>

<template>
  <div id="product">
    <h1 class="titles-components">
      Les massages que je vous propose
    </h1>
    <hr>
      <div class="container">
        <section class="massages">
          <!--Massage étoile-->
          <div class="massage-type">
            <div class="title">
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
            <div class="title">
              <img class="icon" v-bind:src="ayurveda">
              <h3 class="massage-title">
                Ayurvédique
              </h3>
            </div>
            <p>
              Relaxation qui permet de relâcher les tensions nerveuses et musculaires qui entravent la libre circulation de l'énergie dans le corps.
            </p>
          </div>
          <!--Massage suedois-->
          <div class="massage-type">
            <div class="title">
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
            <div class="title">
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
            <div class="title">
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
            <div class="title">
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
.titles-components {
  color: #2f4858;
  font-family: 'Baskerville';
  font-style: italic;
}
p { 
  color: #548086;
}
.massage-title {
  font-weight: 600;
  color: #2f4858;
}
hr {
  width:50%;
  margin: auto;
  margin-bottom: 1em;
}
.massage-type {
  background-color: #eff8f0;
}
p {
  margin-top: 0.5em;
}
/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  #product {
  margin: 1.6em;
}
  .titles-components {
    font-size: 2em;
    text-align: center;
    margin: 0.5em;
    padding-top: 1.5em;
  }
  .massage-type {
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-radius: 1.5em;
    padding: 1.5em;
    margin-bottom: 1.2em;
  }
  .title {
    display: flex;
    align-items: center;
    margin-bottom: 0.5em;
  }
  .icon {
    width: 4em;
    margin-right: 0.9em;
  }
}
/*Médium smartphone device */
@media only screen and (min-width: 681px) {
  #product {
  margin: 1.6em;
  }
  .titles-components {
    font-size: 1.9em;
    text-align: center;
    margin: 0.5em;
    padding-top: 1.5em;
  }
  .massage-type {
    display: flex;
    flex-wrap: wrap;
    border-radius: 1.5em;
    padding: 1.5em;
    margin-bottom: 1.2em;
    height: 13em;
  }
  .title {
    display: flex;
    margin-right: 0.9em;
  }
}
/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  #product {
    margin: 2.5em;
  }
  .titles-components {
    text-align: center;
    margin: 0.5em;
    padding-top: 1.5em;
    font-size: 2.8em;
  }
  hr {
    width: 70%;
  }
  .massage-type {
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-radius: 1.5em;
    padding: 1.5em;
    margin-bottom: 1.2em;
    height: 15em;
  }
  .title {
    display: flex;
    align-items: center;
    margin-bottom: 0.5em;
    font-size: 1.5em;
  }
  .icon {
    width: 3em;
    margin-right: 0.9em;
  }
  p {
    font-size: 1em;
  }
}
/* Medium devices (landscape tablets, 992px and up) */
@media only screen and (min-width: 992px) {
  .titles-components {
    text-align: center;
    margin: 0.5em;
    padding-top: 1.5em;
    font-weight: 500;
    font-size: 2.5em;
  }
  hr {
    width:45%;
  }
  .massages {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  .massage-type {
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-radius: 1.5em;
    padding: 1.5em;
    margin: 1em;
    height: 15em;
    width: 28em;
  }
  .title {
    display: flex;
    align-items: center;
    margin-bottom: 0.5em;
    font-size: large;
  }
  .icon {
    width: 3em;
    margin-right: 0.9em;
  }
  p {
    font-size: 1em;
  }
}
/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  #product {
  margin: 2.5em;
  }
  .titles-components {
    text-align: center;
    margin: 1em;
    padding-top: 1.5em;
    font-weight: 500;
    font-size: 2.5em;
  }
  hr {
  width:35%;
  }
  .massages {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  .massage-type {
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-radius: 1.5em;
    padding: 1.5em;
    margin: 1em;
    height: 16em;
    width: 35em;
  }
  .title {
    display: flex;
    align-items: center;
    margin-bottom: 0.5em;
    font-size: large;
  }
  .icon {
    width: 3em;
    margin-right: 0.9em;
  }
  p {
    font-size: 1em;
  }
}
/* Extra large devices (large laptops and desktops, 1700px and up) */
@media only screen and (min-width: 1700px) {
.titles-components {
  text-align: center;
  margin: 1em;
  padding-top: 1.5em;
  font-weight: 500;
  font-size: 2.8em;
}
hr {
  width:30%;
}
.massages {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.massage-type {
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-radius: 1.5em;
  padding: 1.5em;
  margin: 1em;
  height: 19em;
  width: 50em;
}
.title {
  display: flex;
  align-items: center;
  margin-bottom: 0.5em;
  font-size: x-large;
}
.icon {
  width: 3.5em;
  margin-right: 0.9em;
}
p {
  font-size: 1.2em;
}
}
</style>