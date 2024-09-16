<script>
  export default {
    name : 'app',
    data() {
      return {
        count : 0,
        name : 'Ann',
        name_list : ['Ann', 'Peggy', 'Allen'],
      }
    },
    methods: {
      plaus_Function() {
        return this.count ++
      },
      minus_Function() {
        return this.count --
      },
      name_Function() {
        this.name = this.name_list[this.count]
      }
    }
  }
</script>

<template>
  <p>number : {{ count }}</p>
  <p v-if="count>=0 & count<=2">name : {{ name }}</p>
  <p v-else>no people</p>

  <button v-on:click="minus_Function(), name_Function()"> < </button>
  <button v-on:click="plaus_Function(), name_Function()"> > </button>
</template>

<style scoped>

</style>
