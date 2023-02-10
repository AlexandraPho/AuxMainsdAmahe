<script>
import phone from "@/assets/phoneMail.png";
import adress from "@/assets/adress.png";
import calendar from "@/assets/calendar.png";

export default {
  data() {
      return {
        phone: phone,
        adress: adress,
        calendar: calendar
        };
    },
}
</script>

<template>
  <div id="contactContainer">
    <section class="contact">
      <h1 class="titles-components">
        Contactez-moi pour toutes prestations
      </h1>
      <div class="card">
        <img class="icon" v-bind:src="phone">
        <h3>
          Télephone & E-mail
        </h3>
          <a href="tel:+33769832189">07 69 83 21 89</a>
          <a href="mailto:auxmainsdamahe@outlook.fr?subject=Mail envoyé du site" target="_blank">Envoyez-moi un mail</a>
      </div>
      <div class="card">
        <img class="icon" v-bind:src="adress">
        <h3>
          Adresses
        </h3>
        <p>
          Quincy-Voisin
        </p>
        <p>
          ?????
        </p>
      </div>
      <div class="card">
        <img class="icon" v-bind:src="calendar">
        
        <table>
          <thead>
            <tr>
              <th colspan="2">Horaires</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Lundi</td>
              <td>10h - 16h</td>
            </tr>
            <tr>
              <td>Mardi</td>
              <td>10h - 16h</td>
            </tr>
            <tr>
              <td>Mercredi</td>
              <td>10h - 16h</td>
            </tr>
          </tbody>
        </table>
      </div>
    </section>
  </div>
</template>

<style scoped>
#contactContainer {
  background-color: white;
  text-align: center;
  margin: 2em;
}
.adress {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.titles-components {
  color: #2F4858;
}
.card {
  background-color: #eff8f0;
}
p { 
  color: #548086;
  margin-top: 0.5em;
}
h3,
th{
  color: #2f4858;
  font-weight: 600;
  font-size: large;
}
a {
  text-decoration: none;
}
a,
tr {
  color: #548086;
}

/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  .titles-components {
    text-align: center;
    margin: 1em;
    padding-top: 1.5em;
  }
  .card {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    border-radius: 1.5em;
    padding: 1.5em;
    margin-bottom: 1.2em;
    height: 19em;
    align-items: center;
  }
  .icon {
    width: 4em;
  }
}
</style>
