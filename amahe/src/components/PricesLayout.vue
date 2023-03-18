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
            Le forfait <span class="span">Découverte</span>
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
            Le forfait <span class="span">Détente</span>
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
          <h3> Quelques minutes pour soi</h3>
            <div class="lessTime">
              <p>20 min</p><span>25€</span>
            </div>
            <div class="lessTime">
              <p>30 min</p><span>35€</span>
            </div>
            <div class="lessTime">
              <p>45 min</p><span>50€</span>
            </div>
        </div>
      </section>
      </div>
  </div>
</template>

<style scoped>
#prices {
  margin-top: 2em;
  background-color: #FFFAF1;
  border-radius: 1.5em;
}
.titles-components {
  color: #2f4858;
  font-family: 'Baskerville';
  font-style: italic;
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
  margin: 1.2em;
  width: 5em;
  border-color: #324B4E;
}
span {
  font-weight: bold;
  font-size: large;
  color: #548086;
}
.span {
  font-style: italic;
  font-size: inherit;
}
.condition-pack {
  margin-top: 2em;
}

/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  #prices {
    margin: 5em 1.6em;
  }
  .titles-components {
    font-size: 2em;
    text-align: center;
    margin: 0.6em;
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
/*Smartphone Size*/
@media only screen and (min-width: 681px) {
  #prices {
    margin: 5.5em 1.6em;
  }
  .titles-components {
    font-size: 2em;
    text-align: center;
    margin: 0.6em;
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


/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  #prices {
    margin: 6.5em 2.5em;
  }
  .titles-components {
    text-align: center;
    margin: 1em;
    padding-top: 1.5em;
    font-size: 2.8em;
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
    margin: 1.5em;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
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
    align-items: center;
    font-size: 1em;
    text-align: center;
    width: 20em;
  }
  h3 {
    font-size: 0.9em;
  }
  .package-type p {
    font-size: 1em;
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
    font-size: 0.6em;
  }
  .lessTime,
  .timePrice {
    display: flex;
    align-items: center;
  }
  .lessTime p,
  .timePrice p {
    margin-right: 0.8em;
  }
}

/* Medium devices (landscape tablets, 992px and up) */
@media only screen and (min-width: 900px) {
  #prices {
    margin: 6.5em 2.5em;;
  }
  .titles-components {
    text-align: center;
    margin: 1em;
    padding-top: 1.5em;
    font-size: 2.8em;
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
    margin: 1.5em;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }
  .massage-type,
  .package-type,
  .time-type {
    background-color: white;
    display: flex;
    flex-direction: column;
    border-radius: 1.5em;;
    padding: 1em;
    margin-bottom: 1.2em;
    align-items: center;
    font-size: 1em;
    text-align: center;
    width: 25em;
  }
  h3 {
    font-size: 1em;
  }
  .package-type p {
    font-size: 1em;
  }
  .discovery-package,
  .products {
    margin-bottom: 2em;
  }
  .relax-package,
  .container-prices {
    margin-top: 1.5em;
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
    margin-right: 1.2em;
  }
}

/* Medium devices (landscape tablets, 1200px and up) */
@media only screen and (min-width: 1200px) {
  #prices {
    margin: 6.5em 2.5em;
  }
  .titles-components {
    text-align: center;
    margin: 1em;
    padding-top: 1.5em;
    font-size: 2.8em;
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
    margin: 1.5em;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }
  .massage-type,
  .package-type,
  .time-type {
    background-color: white;
    display: flex;
    flex-direction: column;
    border-radius: 1.5em;;
    padding: 1em;
    margin-bottom: 1.2em;
    align-items: center;
    font-size: 1.2em;
    text-align: center;
    width: 35em;
  }
  h3 {
    font-size: 1em;
  }
  .package-type p {
    font-size: 1em;
  }
  .discovery-package,
  .products {
    margin-bottom: 2em;
  }
  .relax-package,
  .container-prices {
    margin-top: 1.5em;
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
    font-size: 0.6em;
  }
  .lessTime,
  .timePrice {
    display: flex;
    align-items: center;
  }
  .lessTime p,
  .timePrice p {
    margin-right: 1.2em;
  }
}

</style>
