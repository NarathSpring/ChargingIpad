<template>
  <div style="height: 100%">
    <Base />
    <!-- <div class="title"></div> -->
    <div class="content">
      <img src="../assets/2_title.png" alt="" class="title" />
      <img src="../assets/2_qrcode.png" alt="" class="qrcode" />
      <img src="../assets/2_desc.png" alt="" class="desc" />
      <img src="../assets/2_bottom.png" alt="" class="bottom" />
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
.content {
  position: relative;
  display: grid;
  grid-template-rows: 130px 450px 190px 130px;
  justify-items: center;
  align-items: center;
  top: 50%;
  transform: translateY(-50%);
}
.qrcode{
  width: 50%;
}
.bottom {
  
  z-index: -1;
}
</style>
