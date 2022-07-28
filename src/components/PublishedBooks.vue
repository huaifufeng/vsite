<template>
  <div>
    <p>Has Published Books:</p>
    <span>{{publishedBooksMessage}}</span>
    <button @click="setBooks">setBooks</button>
  </div>
</template>

<script>
export default {
  name: "PublishedBooks",
  data() {
    return {
      author :{
        name :"John Doe",
        books : [
            "Vue 2 - Advanced Guide",
            "Vue 3 - Basic Guide",
            "Vue 4 - The Mystery"
        ]
      }
    }
  },
  methods: {
    setBooks() {
      //设置值会更新计算属性
      this.author.books = []
      //赋值也会更新计算属性
       this.publishedBooksMessage = ["new book"]
    }
  },
  computed: {
    publishedBooksMessage : {
      get() {
        return this.author.books.length > 0 ? "Yes" : "No";
      },
      set(books) {
        this.author.books = books
      }
    }
  }
}
</script>

<style scoped>

</style>