<template>
  <div :class="{active : isActive, 'text-danger': hasError }" class="static">
    <p :class="classObject">王子 <span :class="classObjectComputed"></span></p>
    <p :class="[classObject.active ? 'active': '', 'text-danger']">数组</p>
  </div>
</template>

<script>
export default {
  name: "ClassExample",
  data() {
    return {
      isActive : true,
      hasError : false,
      classObject: {
        active: true,
        'text-danger' : true
      }
    }
  },
  computed: {
    classObjectComputed() {
      return {
        active: this.isActive,
        'text-danger':this.hasError
      }
    }
  }
}
</script>

<style scoped>

</style>