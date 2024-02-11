<template>
  <div>
    <h1>Name : {{ form.name }}</h1>
    <v-btn @click="changeName">btn</v-btn>
    <h1>{{ showFullName }}</h1>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      fname: 'panwa',
      lname: 'Mu',
      age: 0,
      form: { name: 'test', age: 0 },
    }
  },
  methods: {
    changeName() {
      this.form.name = 'panwa'
    },
  },
  computed: {
    showFullName() {
      return this.fname + ' ' + this.lname
    },
  },
}
</script>
