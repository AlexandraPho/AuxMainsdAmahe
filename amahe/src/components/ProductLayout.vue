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
  <div id="contactContainer">
    <section class="contact">
      <h1 class="titles-components">
        Contactez-moi pour toutes prestations
      </h1>
      <hr>
      <div class="all-cards">
        <div class="card">
          <img class="icon" alt="icon" v-bind:src="contact">
          <!--<h3>
            Télephone & E-mail
          </h3>-->
          <div class="card-contact">
            <a href="tel:+33769832189"><img class="sub-icon" alt="icon" v-bind:src="phone">07 69 83 21 89</a>
            <a href="mailto:auxmainsdamahe@outlook.fr?subject=Mail envoyé du site" target="_blank"><img class="sub-icon" alt="icon" v-bind:src="mail">Envoyez-moi un mail</a>
          </div>
        </div>
        <div class="card">
          <img class="icon" alt="icon" v-bind:src="adress">
          <!--<h3>
            Adresses
          </h3>-->
          <p>
            Quincy-Voisins
          </p>
          <p>
            Croissy-Beaubourg
          </p>
        </div>
        <div class="card">
          <img class="icon" alt="icon" v-bind:src="calendar">
          
          <table>
            <thead>
              <!--<tr>
                <th colspan="2">Horaires</th>
              </tr>-->
            </thead>
            <tbody>
              <tr>
                <td>Lundi </td>
                <td>10h - 19h</td>
              </tr>
              <tr>
                <td>Mardi </td>
                <td>10h - 19h</td>
              </tr>
              <tr>
                <td>Jeudi </td>
                <td>10h - 19h</td>
              </tr>
              <tr>
                <td class="day">Vendredi </td>
                <td>10h - 19h</td>
              </tr>
            </tbody>
          </table>
          <p>Le weekend sur demande</p>
        </div>
    </div>
    </section>
  </div>
</template>

<style scoped>
#contactContainer {
  background-color: white;
  text-align: center;
}
.titles-components {
  font-family: 'Baskerville';
  font-style: italic;
}
hr {
  width:50%;
  margin: auto;
  margin-bottom: 1em;
}
.adress {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.adress {
  display: flex;
    flex-direction: column;
    align-items: center;
}
.titles-components,
h3,
th{
  color: #2F4858;
}
.card {
  background-color: #eff8f0;
}
.card-contact {
  display: flex;
  flex-direction: column;
}

p { 
  margin-top: 0.5em;
}
a {
  text-decoration: none;
  display: flex;
  flex-direction: column;
  align-items: center;
  border: 1px none;
  border-radius: 1em;
  padding: 0.4em;
  box-shadow: 5px 5px 15px #c9cbc9;
  margin-bottom: 0.7em;
}
a,
tr,
p {
  color: #548086;
}
td {
  text-align: center;
}
.day {
  padding-right: 1.5em;
}
table {
  margin-top: 1.2em;
}

/*Smartphone Size*/
@media only screen and (max-width: 680px) {
  #contactContainer {
    margin: 1.6em;
  }
  .titles-components {
    font-size: 2em;
    text-align: center;
    margin: 0.6em;
    padding-top: 1.5em;
  }
  .all-cards {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .card {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    border-radius: 1.5em;
    padding: 1.2em;
    margin-bottom: 1.2em;
    height: 19em;
    align-items: center;
  }
  .icon {
    width: 4em;
  }
  .sub-icon {
    width: 2em;
  }
  p, td {
    font-size: 1.1em;
  }
}


/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  #contactContainer {
    margin: 2.5em;
  }
  .titles-components {
    text-align: center;
    margin: 1em;
    padding-top: 1.5em;
    font-size: 2.8em;
  }
  .all-cards {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .card {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    border-radius: 1.5em;
    padding: 1.2em;
    margin-bottom: 1.2em;
    height: 19em;
    align-items: center;
  }
  .card-contact {
    display: inline-flex;
    justify-content: space-evenly;
  }
  .icon {
    width: 4em;
  }
  .sub-icon {
    width: 1.8em;
  }
  th,
  tr {
    font-size: 1em;
    margin-bottom: 0.5em;
  }
  a,
  p,
  td {
    font-size: 1.2em;
  }
  a {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
}

/* Medium devices (landscape tablets, 800px and up) */
@media only screen and (min-width: 800px) {
  .all-cards {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }
  .card {
    width: 16em;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    border-radius: 1.5em;
    padding: 1.2em;
    margin-bottom: 1.2em;
    height: 24em;
    align-items: center;
  }
}
</style>

