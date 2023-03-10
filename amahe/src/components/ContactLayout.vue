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
      <div class="contact-card"> 
                <div class="contact-infos">
                    <div class="item">
                        <img class="icon" alt="icon" v-bind:src="adress">
                        <div class="text">
                            <p> Quincy-Voisins, 77860</p>
                            <p> Croissy-Beaubourg, 77183</p>
                        </div>                          
                    </div>
                    <div class="item">
                      <img class="sub-icon" alt="icon" v-bind:src="phone">
                        <div class="text">
                            <a href="tel:+33769832189">07 69 83 21 89</a>
                        </div>                          
                    </div>
                    <div class="item">
                      <img class="sub-icon" alt="icon" v-bind:src="mail">
                        <div class="text">
                          <a href="mailto:auxmainsdamahe@outlook.fr?subject=Mail envoyé du site" target="_blank">Envoyez-moi un mail</a>
                        </div>
                    </div>
                    <div class="item">
                      <img class="icon" alt="icon" v-bind:src="calendar">
                        <div class="text">
                          <table>
                            <thead>
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
                </div>                  
            </div> 
    </section>
    <div id="map" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; z-index: -1;">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d20983.21825499983!2d2.8406314344982495!3d48.898199435308435!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47e8a6e446e559b9%3A0x40b82c3688c4ed0!2s77860%20Quincy-Voisins%2C%20France!5e0!3m2!1sfr!2sus!4v1678459827973!5m2!1sfr!2sus" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>    </div>
  </div>
</template>

<style scoped>
#contactContainer {
  background-color: white;
  text-align: center;
}
.contact {
  border-radius: 1.5em;
  display: flex;
  flex-direction: column;
  align-items: center;
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
.titles-components,
h3,
th{
  color: #2F4858;
}
p { 
  margin-top: 0.5em;
}
.contact-infos {
  display: flex;
  flex-direction: column;
  border: 1px none;
  padding: 1.8em;
  background-color: #eff8f0;
  border-radius: 1.5em;
  box-shadow: 5px 5px 15px #c9cbc9;
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
  .contact {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .conatct-card {
    width: 20em;
    display: flex;
    justify-content: center;
  }
  .contact-infos {
    width: 20em;
  }
  .item {
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
  }
  .text {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    margin-left: 0.5em;
  }

  .titles-components {
    font-size: 2em;
    text-align: center;
    margin: 0.6em;
    padding-top: 1.5em;
  }
  .icon {
    width: 2.5em;
  }
  .sub-icon {
    width: 2em;
  }
  p, td {
    font-size: 1em;
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
@media only screen and (min-width: 900px) {
  .contact-card {
    display: flex;
    justify-content: center;
  }
  .contact-infos {
    display: flex;
    flex-direction: column;
  }
  .item {
    display: flex;
  }
}
</style>
