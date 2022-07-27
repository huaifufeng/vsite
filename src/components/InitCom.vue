<!--- 组件的入口组件 --->
<template>
  <counter-s></counter-s>
  <attr-bind></attr-bind>
  <event-handling></event-handling>
  <two-way-binding></two-way-binding>
</template>

<script>
import CounterS from "@/components/CounterS";
import AttrBind from "@/components/AttrBind";
import EventHandling from "@/components/EventHandling";
import TwoWayBinding from "@/components/TwoWayBinding";

export default {
  name: "InitCom",
  components: {TwoWayBinding, EventHandling, AttrBind, CounterS}
}
</script>

<style scoped>

</style>