<!--- 组件的入口组件 --->
<template>
  <ModelExample title="小王子呀"></ModelExample>
  <for-example></for-example>
  <if-example></if-example>
  <counter-s></counter-s>
  <attr-bind></attr-bind>
  <event-handling></event-handling>
  <two-way-binding></two-way-binding>
  <conditional-rendering></conditional-rendering>
  <list-rendering></list-rendering>
  <published-books></published-books>
  <watch-example></watch-example>
  <class-example></class-example>
</template>

<script>
import CounterS from "@/components/CounterS";
import AttrBind from "@/components/AttrBind";
import EventHandling from "@/components/EventHandling";
import TwoWayBinding from "@/components/TwoWayBinding";
import ConditionalRendering from "@/components/ConditionalRendering";
import ListRendering from "@/components/ListRendering";
import PublishedBooks from "@/components/PublishedBooks";
import WatchExample from "@/components/WatchExample";
import ClassExample from "@/components/ClassExample";
import IfExample from "@/components/IfExample";
import ForExample from "@/components/ForExample";
import ModelExample from "@/components/ModelExample";

export default {
  name: "InitCom",
  components: {
    ModelExample,
    ForExample,
    IfExample,
    ClassExample,
    WatchExample,
    PublishedBooks, ListRendering, ConditionalRendering, TwoWayBinding, EventHandling, AttrBind, CounterS}
}
</script>

<style scoped>
div {
  max-width: 200px;
  text-align: center;
  margin: 2px auto;
}
</style>