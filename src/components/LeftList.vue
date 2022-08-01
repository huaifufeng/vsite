<template>
  <div class="left">
    <left-top></left-top>
    <left-down></left-down>
  </div>
</template>

<script>
import LeftTop from "@/components/LeftTop";
import LeftDown from "@/components/LeftDown";
export default {
  name: "LeftList",
  components: {LeftDown, LeftTop}
}
</script>

<style scoped>
.left{
  background-color: #42b983;
  width: 20%;
  min-width: 200px;
  height: 100%;
  position: fixed;
}


</style>