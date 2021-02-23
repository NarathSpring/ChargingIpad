<template>
  <div class="base">
    <img src="../assets/1_mask.png" alt="" class="top" />
  </div>
</template>

<script lang="ts">
import { Vue } from "vue-property-decorator";

export default class Base extends Vue {}
</script>

<style scoped>
.base {
  position: absolute;
  background: url("../assets/background.png");
  background-size: cover;
  height: 100%;
  width: 100%;
}
.top {
  width: 100%;
  position: absolute;
  /* top: 30px; */
  left: 0;
  right: 0;
  margin: 0 auto;
  z-index: 999;
}
</style>
