<template>
  <div>Counter : {{counter}}</div>
  <button v-bind:disabled="isDisabled">disabled</button>
</template>

<script>
export default {
  name: "CounterS",
  data() {
    return {
      counter : 10,
      isDisabled : true
    }
  },
  mounted() {
    setInterval(() => {
      this.counter++
    }, 1000)
  }
}
</script>