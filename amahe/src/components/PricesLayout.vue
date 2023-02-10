<script>
export default {
}
</script>

<template>
  <div id="prices">
    <h1 class="titles-components">
      Je choisi le temps qui me fait plaisir
    </h1>
    <div class="container">
      <section class="prices">
        <!--Type of massage-->
        <div class="massage-type">
          <h3>Le temps d'un massage</h3>
          <p class="products">
            Massage étoile<br>
            Ayurvédique<br>
            Suédois<br>
            Shiatsu<br>
            Balinais<br>
            Réflexologie plantaire douce
          </p>
          <hr>
          <div class="container-prices">
            <!--Price for 60'-->
            <div class="timePrice">
              <p>60 minutes de massage</p><span>65€</span>
            </div>
            <!--Price for 90'-->
            <div class="timePrice">
              <p>90 minutes de massage</p><span>95€</span>
            </div>
          </div>
        </div>
        <!--Package-->
      <div class="package-type">
        <h3>Les forfaits bien-être *</h3>
        <!--Discovery package-->
        <div class="discovery-package">
          <p>
            Le forfait découverte
          </p>
          <p>
            3 massages d'une heure
          </p>
          <div>
            <span>
              165€&nbsp;
            </span>
            <span class="condition">
              au lieu de 195€&nbsp;
            </span><br>
            <small class="subscription">
              Valable 6 mois à partir de la date de souscription
            </small>
          </div>
        </div>
        <hr>
        <div class="relax-package">
          <!--Relax package-->
          <p>
           Détente
          </p>
          <p>
            5 massages d'une heure
          </p>
          <div>
            <span>
              275€&nbsp;
            </span>
            <span class="condition">
              au lieu de 325€&nbsp;
            </span><br>
            <small class="subscription">
              Valable 8 mois à partir de la date de souscription
            </small>
          </div>
          <div class="condition-pack">
              <strong>*</strong> À vous de combiner les massages que vous souhaitez
          </div>
        </div>
      </div>

        <!--Less time-->
        <div class="time-type">
          <h3> Vous avez peu de temps ou 
            bien vous souhaitez privilégier juste une zone.
            Je vous propose un massage adapté à vos besoins.</h3>
            <div class="lessTime">
              <p>20 min</p><span>25€</span>
            </div>
            <div class="lessTime">
              <p>30 min</p><span>35€</span>
            </div>
            <div class="lessTime">
              <p>45 min</p><span>45€</span>
            </div>
        </div>
      </section>
      </div>
  </div>
</template>

<style scoped>
#prices {
  margin-top: 2em;
  background-color: #F8F1E3;
  border-radius: 1.5em;
}
.titles-components {
  color: #2f4858;
}
h3,
p,
.subscription,
.condition-pack {
  color: #2f4858;
}
p {
  color: #548086;
}
h3 {
  font-weight: bold;
  text-transform: uppercase;
  margin-bottom: 0.5em;
}
hr {
  margin: auto;
  width: 5em;
  border-color: #324B4E;
}
span {
  font-weight: bold;
  font-size: large;
  color: #548086;
}
/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  .titles-components {
    text-align: center;
    margin: 1em;
    padding-top: 1.5em;
  }
  .container {
    padding-bottom: 2em;
  }
  .container-prices {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  .prices {
    margin: 2em;
  }
  .massage-type,
  .package-type,
  .time-type {
    background-color: white;
    display: flex;
    flex-direction: column;
    border-radius: 1.5em;;
    padding: 1.2em;
    margin-bottom: 1.2em;
  }
  .package-type p {
    font-size: large;
  }
  .discovery-package,
  .products {
    margin-bottom: 2em;
  }
  .relax-package,
  .container-prices {
    margin-top: 2em;
  }
  .price {
    width: 9em;
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-radius: 0.7em;
    margin-bottom: 1.2em;
    padding: 1.5em;
  }
  .condition {
    font-weight: normal;
  }
  .subscription {
    font-style: italic;
    font-weight: normal;
    font-size: small;
  }
  .condition-pack {
    font-weight: normal;
    font-size: 0.9em;
  }
  .lessTime,
  .timePrice {
    display: flex;
    align-items: center;
  }
  .lessTime p,
  .timePrice p {
    margin-right: 1em;
  }
}
</style>