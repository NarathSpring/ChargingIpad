<template>
  <swiper ref="mySwiper" :options="swiperOptions" class="swiper-container">
    <swiper-slide class="slide1 "><Slide1 /></swiper-slide>
    <swiper-slide class="slide2 "><Slide2 /></swiper-slide>
    <swiper-slide class="slide3 "><Slide3 /></swiper-slide>
    <swiper-slide class="slide3 "><Slide4 /></swiper-slide>
    <swiper-slide class="slide3 "><Slide5 /></swiper-slide>
  </swiper>
  
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import { SwiperOptions } from "swiper";
import Slide1 from "./Slide1.vue";
import Slide2 from "./Slide2.vue";
import Slide3 from "./Slide3.vue";
import Slide4 from "./Slide4.vue";
import Slide5 from "./Slide5.vue";

@Component({
  components: { Slide1, Slide2, Slide3, Slide4, Slide5 }
})
export default class ChargingIpad extends Vue {
  swiperOptions: SwiperOptions = {
    effect: "fade",
    direction: "vertical",
    speed: 300,
    freeMode: false
  };
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
swiper-slide {
  height: 300px;
}
.slide1 {
  background: white;
}
.slide2 {
  background: white;
}
.slide3 {
  background: white;
}
.slide4 {
  background: white;
}
.slide5 {
  background: white;
}
.swiper-container {
  width: 100%;
  height: 100%;
}
</style>
