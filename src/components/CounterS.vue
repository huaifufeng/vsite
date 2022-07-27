<template>
  Counter : {{counter}}
</template>

<script>
export default {
  name: "CounterS",
  data() {
    return {
      counter : 10
    }
  },
  mounted() {
    setInterval(() => {
      this.counter++
    }, 1000)
  }
}
</script>