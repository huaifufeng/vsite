<template>
  <left-list></left-list>
  <right-content></right-content>
</template>

<script>
import LeftList from "@/components/LeftList";
import RightContent from "@/components/RightContent";

export default {
  name: 'App',
  components: {
    RightContent,
    LeftList,
  }
}
</script>

<style>
body {
  margin: 0;
}
#app {
  position: relative;
}
</style>
