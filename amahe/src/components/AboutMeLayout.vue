<script>
import office from "@/assets/office.jpeg";

export default {
  data() {
      return {
        office: office,
      
        };
    },
}
</script>

<template>
  <div id="aboutMe">
    <img class="office" v-bind:src="office"> 
    <!--<h2 class="titles-components">
      A propos de moi
    </h2>-->
      <section class="block-container">
        <div class="text">
          <h3 class="titles">
            À l'écoute de votre corps
          </h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec eu massa a turpis commodo fermentum. Ut euismod leo et lacinia mattis. Integer quis risus quam. Donec dui libero, sollicitudin ultricies mattis eu, tincidunt bibendum sapien. Sed iaculis, ex quis pellentesque luctus, massa dolor ultricies mauris, a feugiat est quam at nisi. In mollis, mi eu tincidunt cursus, ligula massa rhoncus odio, sed auctor velit tortor at quam. Cras venenatis ornare massa molestie malesuada. Integer pretium dolor eu hendrerit laoreet. Phasellus in orci pellentesque ligula tristique tempus. Fusce eleifend arcu sed velit auctor facilisis. Vivamus sit amet ipsum nulla. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.
          </p>
        </div>
      </section>
  </div>
</template>
