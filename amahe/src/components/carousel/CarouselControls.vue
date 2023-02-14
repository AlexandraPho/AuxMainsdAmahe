<script>
  import left from "@/assets/left.png";
  import right from "@/assets/right.png";

  export default {
    data() {
        return {
        left: left,
        right: right,
        }
    },
   
    emits: ["prev", "next"], 
  };
  </script>

<template>
    <!-- in vue 2.x you need wrap these buttons in a div -->
    <button class="carousel-control left" @click="$emit('prev')"><img v-bind:src="left" :alt="prev" class="prev"></button>
    <button class="carousel-control right" @click="$emit('next')"><img v-bind:src="right" :alt="next" class="next"></button>
  </template>

  <style scoped>
  .carousel-control {
    background-color: #548086a2;
    border: none;
    display: inline-block;
    position: absolute;
    height: 45px;
    width: 30px;
    top: calc(50% - 25px);
    color: #f3f3f3;
    cursor: pointer;
  }
  .left {
    left: 0;
  }
  .right {
    right: 0;
  }
  .left,
  .right {
    padding: 0;
  }
  .prev,
  .next {
    width: 2.2em;
  }
  </style>