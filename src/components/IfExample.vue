<template>
  <div>
    <h1 v-if="Math.random() > 0.5">Vue is awesome</h1>
    <h1 v-else>Oh no</h1>

    <h2 v-show="awesome">Vue is show </h2>
  </div>
</template>

<script>
export default {
  name: "IfExample",
  data() {
    return {
      awesome: true
    }
  }
}
</script>

<style scoped>

</style>