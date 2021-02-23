<template>
  <div id="app">
    <ChargingIpad />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import ChargingIpad from "./components/ChargingIpad.vue";
import Slide1 from "./components/Slide1.vue";
import Slide2 from "./components/Slide2.vue";
import Slide3 from "./components/Slide3.vue";
import Slide4 from "./components/Slide4.vue";
import Slide5 from "./components/Slide5.vue";

@Component({
  components: {
    ChargingIpad,
    Slide1,
    Slide2,
    Slide3,
    Slide4,
    Slide5
  }
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
}
</style>
