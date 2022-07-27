<template>
  <div>
    <span v-if="seen">现在你看到我了</span>
  </div>
</template>

<script>
export default {
  name: "ConditionalRendering",
  data() {
    return {
      seen : true
    }
  }
}
</script>

<style scoped>

</style>