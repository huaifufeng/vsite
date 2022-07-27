<template>
  <div id="bind-attribute">
    <span v-bind:title="message">
        鼠标悬停几秒钟查看此处动态绑定的提示信息！
    </span>
  </div>
  <counter-s></counter-s>
</template>

<script>
  import CounterS from "@/components/CounterS";

  export default {
    name: "AttrBind",
    components: {CounterS},
    data() {
      return {
        message :  "You loaded this page on " + new Date().toLocaleString()
      }
    }
  }

</script>