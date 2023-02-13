<script>
import left from "@/assets/left.png";
import right from "@/assets/right.png";

export default {
    emits: ['prev', 'next'],

    data() {
      return {
        left: left,
        right: right,
      };

    },
}
</script>


<template>
    <button class="carousel-control left" @click="$emit('prev')"><img class="left-chevron" v-bind:src="left"></button>
    <button class="carousel-control right" @click="$emit('next')"><img class="right-chevron" v-bind:src="right"></button>

</template>

<style scoped>
.carousel-control {
    background-color:rgba(84, 129, 135, 0.568);
    border: none;
    display: inline-block;
    position: absolute;
    height: 38px;
    width: 32px;
    top: calc(50% - 25px);
    color: #eff8f0;
    cursor: pointer;
}
.left {
    left: 0;
}
.right {
    right: 0;
}
.left-chevron,
.right-chevron {
    width: 2em;
}
</style>