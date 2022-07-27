<!--- 组件的入口组件 --->
<template>
  <counter-s></counter-s>
  <attr-bind></attr-bind>
  <event-handling></event-handling>
  <two-way-binding></two-way-binding>
  <conditional-rendering></conditional-rendering>
  <list-rendering></list-rendering>
</template>

<script>
import CounterS from "@/components/CounterS";
import AttrBind from "@/components/AttrBind";
import EventHandling from "@/components/EventHandling";
import TwoWayBinding from "@/components/TwoWayBinding";
import ConditionalRendering from "@/components/ConditionalRendering";
import ListRendering from "@/components/ListRendering";

export default {
  name: "InitCom",
  components: {ListRendering, ConditionalRendering, TwoWayBinding, EventHandling, AttrBind, CounterS}
}
</script>

<style scoped>
div {
  max-width: 200px;
  text-align: center;
  margin: 2px auto;
}
</style>