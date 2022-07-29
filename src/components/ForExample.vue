<template>
  <div>
    <ul>
      <li v-for="(item, index) of list.items" :key="item.message">
        <!---可以访问父级的属性--->
        {{parentMessage}} {{ index }} {{item.message}}
      </li>
      <li v-for="(item, name, index) in obj">
        {{name}} {{item}} {{index}}
      </li>
      <!--- 计算属性不适用时，使用方法   嵌套for循环--->
      <li v-for="n in evenNumbers">
        {{n}}
      </li>
      <li v-for="n in 10">
        {{n}}
      </li>
      <template v-for="item in list.items">
        <li>{{item.message}}</li>
        <li class="divider" role="presentation"></li>
      </template>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ForExample",
  data() {
    return {
      parentMessage: "parent",
      list: {
        items : [
          {message : "first"}, {message : "second"}
        ]
      },
      obj: {
        title: 'How to do list in Vue',
        'author': "Jane Doe",
        "publishedAt": "2022-03-03"
      },
      numbers: [1,2,3,4,5]
    }
  },
  computed: {
    evenNumbers() {
      return this.numbers.filter(number => number % 2 === 0)
    }
  }
}
</script>

<style scoped>

</style>