<template>
  <div style="height: 100%">
    <Base />
    <!-- <div class="title"></div> -->
    <img src="../assets/5_end.png" alt="" class="title" />
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
}
.title {
  top: 50%;
  transform: translateY(-50%);
}
</style>
