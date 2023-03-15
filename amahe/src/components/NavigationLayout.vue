<script>
import logo from "@/assets/fleur.svg";
import menu from "@/assets/menu.png";

  export default {
    data() {
      return {
        showMobileMenu: false,
        logo: logo,
        menu: menu,
        };
    },
    methods: {
      showMenu() {
        this.showMobileMenu = !this.showMobileMenu;
      },
      closeMenu() {
        this.showMobileMenu = false;
      },
    },
  };
</script>

<template>
  <header id="header">
      <div class="logo-container">
          <!--LOGO-->
          <a href ="#main" class="link-header">
          <img class="logo" v-bind:src="logo">
          <div class="text-container">
              <span class="first-part">Aux mains </span>
              <span class="second-part">d'Amahé</span>
          </div>
        </a>
          <!--Hamburger icon with click method-->
          <img class="img-burger-menu" v-bind:src="menu" @click="showMenu()"> 
      </div>
      <!--Menu content-->
      <nav class="nav-content" :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'">
        <ul class="nav-items">
          <a href="#aboutMe" @click="closeMenu"><li>À propos de moi</li></a>
          <a href="#product" @click="closeMenu"><li>Les massages</li></a>
          <a href="#prices" @click="closeMenu"><li>Les tarifs</li></a>
        </ul>
        <button class="btn-form"><a href="#contactContainer" class="button" @click="closeMenu">Prendre rendez-vous</a></button>
      </nav>
  </header>
</template>


<style scoped>

#header{
    background-color: white;
    width: 100%;
    position: fixed;
    z-index:1;
    box-shadow: rgba(10, 83, 32, 0.1) 0px 10px 10px;
  }
  .link-header {
    color: #2F4858;
  }
  .nav-content {
    display: flex;
    justify-content: space-between;
    padding: 5px 10px;
    align-items: flex-start;
  }
  .nav-items {
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    margin: 0;
    padding: 0;
  }
  li {
    color: #2F4858;
    padding: 0 10px;
  }
  li:hover {
    color: #89B68E;
  }
  a {
    text-decoration: none;
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
  .btn-form a {
    position: relative; 
    z-index: 1;
    color: #2F4858;
  }
  .btn-form:after {
    content: "";
    position: absolute;
    left: 0;
    top: 0;
    height: 400%;
    width: 140%;
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
    color: #2F4858;
  }
  .logo {
      filter: blur(0.4px);
      transform: rotate(-15deg);
  }
  .first-part {
    font-weight: 600;
  }
  .second-part {
    font-family: 'baskerville';
    font-style: italic;
    margin-left: 1.4em;
    font-size: 1.4em;
  }

  /*Mobile version - hidden hamburger menu*/
  @media screen and (max-width: 767px) {
    #header {
      display: flex;
      justify-content: space-around;
      flex-direction: column;
    }
    .logo-container {
      padding: 1.2em;
      display: flex;
      position: relative;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      width: 7em;
      margin-left: 3em;
    }
    .first-part{
      font-size: 1.3;
    }
    .second-part {
      font-size: 1.2em;
    }
    .text-container {
      display: flex;
      flex-direction: column;
      position: absolute;
      bottom: 2em;
    }
    .img-burger-menu {
      width: 3em;
      height: 3em;
      padding: 5px;
    }
    .nav-content {
      flex-direction: column;
      align-items: center;
      z-index: 100;
      position: relative;
      transition: all 0.2s ease-out;
      margin: 5px;
    }
    .open-menu {
      opacity: 1;
      height: 250px;
    }
    .closed-menu {
      opacity: 0;
      height: 0;
      padding: 0;
    }
    .nav-items {
      flex-direction: column;
      display: flex;
      align-items: center;
    }
    li {
      margin: 10px;
    }
    .btn-form {
      margin-bottom: 1.5em;
    }
    .btn-form:after {
      height: 400%;
      width: 140%;
    }
  }
  
  /*Tablet version*/
  @media screen and (min-width: 768px) {
    #header {
      display: flex;
      justify-content: space-around;
      flex-direction: column;
    }
    .logo-container {
      padding: 1.5em;
      display: flex;
      position: relative;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      width: 10em;
      margin-left: 4.8em;
    }
    .first-part{
      font-size: 1.5em;
    }
    .second-part {
      font-size: 1.8em;
    }
    .text-container {
      display: flex;
      flex-direction: column;
      position: absolute;
      bottom: 2.5em;
    }
    .img-burger-menu {
      width: 4.5em;
      height: 4.5em;
      padding: 10px;
    }
    .nav-content {
      flex-direction: column;
      align-items: center;
      z-index: 100;
      position: relative;
      transition: all 0.2s ease-out;
      margin: 5px;
    }
    .open-menu {
      opacity: 1;
      height: 300px;
    }
    .closed-menu {
      opacity: 0;
      height: 0;
      padding: 0;
    }
    .nav-items {
      flex-direction: column;
      display: flex;
      align-items: center;
      font-size: larger;
    }
    li {
      margin: 10px;
      font-size: larger;
    }
    .btn-form {
      margin-bottom: 0.8em;
      font-size: larger;
    }
    .btn-form:after {
      height: 400%;
      width: 140%;
    }
  }
  
  /*Desktop version*/
  @media screen and (min-width: 1200px) {
    #header{
      width: 100%;
      height: 8em;
      display: flex;
      flex-wrap: wrap;
      align-content: stretch;
    }
    .first-part,
    .second-part{
      font-size: 1.8em;
    }
    .header-logo {
      width: 6em;
      padding: 15px;
    }
    .img-burger-menu {
      display: none;
    }
    .nav-content {
      opacity: 1;
      display: flex;
      flex-direction: row;
    }
    .nav-items {
      flex-direction: row;
      margin-right: 5em;
    }
    li {
      margin: 10px;
      font-size: 1.1em;
    }
    .btn-form {
      margin-right: 1.2em;
      margin-bottom: 0;
    }
  }
 /* @media screen and (min-width: 1500px) {
    .nav-items{
      margin-right: 9em;
    }
  }
  @media screen and (min-width: 1860px) {
    .nav-items{
     margin-right: 16em;
    }
  }
  @media screen and (min-width: 2050px) {
    .nav-items{
     margin-right: 25em;
    }
  }*/
</style>