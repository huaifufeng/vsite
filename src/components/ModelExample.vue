<template>
  <div>
    <input v-model="message" placeholder="edit me" />
    <p>Message is {{title}} {{message}}</p>

    <span>Multiline message is:</span>
    <p style="white-space: pre-line">{{message}}</p>
    <br/>
    <textarea v-model="message" placeholder="add multiple line">xiaohazi</textarea>

    <input type="checkbox" id="checked1" value="checked1" v-model="checkedNames"/>
    <label for="checked1">{{checkedNames}}</label>
    <input type="checkbox" id="checked2" value="checked2" v-model="checkedNames"/>
    <label for="checked2">{{checkedNames}}</label>

    <input type="radio" id="one" value="one" v-model="picked"/>
    <label for="one">one</label>
    <input type="radio" id="two" value="two" v-model="picked">
    <label for="two">two</label>
    <span>{{picked}}</span>
    <br>
  </div>
</template>

<script>
export default {
  name: "ModelExample",
  emits: {
    click: null,
    submit: ({email, password}) => {
      if (email && password) {
        return true;
      } else {
        console.warn('Invalid submit event payload!')
        return false;
      }
    }
  },
  methods: {
    submitForm(email, password) {
      this.$emit('submit', {email, password})
    }
  },
  props: {
    title: {
      type: String,
      default: ""
    }
  },
  data() {
    return {
      message: '王子',
      checkedNames: [],
      picked: ''
    }
  }
}
</script>

<style scoped>

</style>