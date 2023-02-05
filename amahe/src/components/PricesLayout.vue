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
          <p>
            Massage étoile<br>
            Ayurvédique<br>
            Suédois<br>
            Shiatsu<br>
            Balinais<br>
            Réflexologie plantaire douce
          </p>
        </div>
        <div class="container-prices">
          <!--Price for 60'-->
         
            <p>
              60 minutes de massage
            </p>
            <span>
              65 euros
            </span>

          <!--Price for 90'-->
          
            <p>
              90 minutes de massage
            </p>
            <span>
              95 euros
            </span>

        </div>

        <!--Package-->
        <div class="package-type">
          <h3>Les forfaits bien-être *</h3>
          <!--Discovery package-->
          <p>
            Le forfait découverte
          </p>
          <p>
            3 massages d'une heure
          </p>
          <div>
            <span>
              165 euros
            </span>
            <span class="condition">
              au lieu de 195 euros
            </span>
            <span class="souscription">
              Valable 6 mois à partir de la date de souscription
            </span>
          </div>
          <!--Relax package-->
          <p>
            Le forfait détente
          </p>
          <p>
            5 massages d'une heure
          </p>
          <div>
            <span>
              275 euros
            </span>
            <span class="condition">
              au lieu de 325 euros
            </span>
            <span class="souscription">
              Valable 8 mois à partir de la date de souscription
            </span>
          </div>
          <span>
              <strong>*</strong> À vous de combiner les massages que vous souhaitez
            </span>
        </div>

        <!--Less time-->
        <div class="time-type">
          <h3> Vous avez peu de temps ou 
            bien vous souhaitez privilégier juste une zone.
            Je vous propose un massage adapté à vos besoins.</h3>
          <span>
            20 min - 25€
          </span>
          <span>
            30 min - 35€
          </span>
          <span>
            45 min - 45€
          </span>
        </div>
      </section>
      </div>
  </div>
</template>

<style scoped>
.price {
    background-color: #d1e4d4;
  }
h3 {
  font-weight: bold;
  text-transform: uppercase;
  color: #334435; /*dark green*/
  margin-bottom: 0.5em;
}
span {
  font-weight: bold;
  font-size: large;
}
/*Smartphone Size*/
@media only screen and (max-width: 680px) {

.titles-components {
  text-align: center;
}
.massage-type,
.package-type,
.time-type {

}
.container-prices {
  display: flex;
  justify-content: space-between;
  text-align: center;
}
.prices {
  margin: 1.5em;
}
.massage-type,
.package-type,
.time-type {
display: flex;
flex-direction: column;

text-align: center;
border-radius: 0.7em;
background-color: #eff8f0;
padding: 1em;
margin-bottom: 1.2em;
 }
.price {
  width: 9em;
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-radius: 0.7em;
  margin-bottom: 1.2em;
  padding: 1em;
}

}
</style>