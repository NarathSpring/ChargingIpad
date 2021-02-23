<template>
  <div style="height: 100%">
    <Base />
    <div class="content">
      <img src="../assets/1_title.png" alt="" class="title" />
      <img src="../assets/1_main.png" alt="" class="main" />
      <div class="bottom">
        <img src="../assets/1_circle.png" alt="" class="circle" />
        <img src="../assets/1_button.png" alt="" class="button" />
      </div>
    </div>
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
img {
  position: relative;
  margin: 0 auto;
  left: 0;
  right: 0;
  top: 0;
}
.content {
  position: relative;
  height: 100%;
  top: 0;
}
.title {
  width: 65%;
  top: 7%;
}
.main {
  top: 12%;
}
.bottom {
  position: relative;
  top: 270px;
  height: 100%;
}
.bottom > img {
  position: absolute;
  bottom: 0;
}
.circle {
  top: -45px;
  width: 40%;
}
.button {
  z-index: 999;
}
</style>
