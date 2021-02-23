<template>
  <div style="height: 100%">
    <Base />
    <!-- <div class="title"></div> -->
    <img src="../assets/4_title.png" alt="" class="title" />
    <img src="../assets/4_g1.png" alt="" class="bottom" />
    <p class="num">98%</p>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import Base from "./Base.vue";

@Component({
  components: {
    Base
  }
})
export default class Slide1 extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@font-face {
  font-family: cc;
  src: url("../assets/YouSheBiaoTiHei-2.ttf");
}
img {
  position: relative;
  margin: 0 auto;
  left: 0;
  right: 0;
}
.title {
  top: 7%;
}
.bottom {
  position: absolute;
  bottom: 0;
  z-index: 999;
}
.num {
  font-family: cc;
  font-size: 110px;
  color: #f3e228;
  z-index: 999;
  position: absolute;
  top: 15%;
  left: 0;
  right: 0;
  margin: 0 auto;
}
</style>
