<template>
  <div class="about">
    <h1>This is the display page:</h1>
    <img id="screen" src="../assets/example.jpg" />
  </div>
</template>

<style lang="css" scoped>
@import "~viewerjs/dist/viewer.css";
</style>

<script>
import Viewer from "viewerjs";

export default {
  mounted() {
    console.log('About.vue is mounted');
    /*let viewer = */new Viewer(this.$el.querySelector("#screen"), {
      
      viewed() {
        console.log("hellow from viewer");
      }
    });
  }
};
</script>