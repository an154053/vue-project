<script>
  export default {
    name : 'app',
    data() {
      return {
        x: 100,
        y: 20,
      }
    },
    methods: {
      myFunction() {
        return this.x * this.y
      }
    }
  }
</script>

<template>
  x : {{ x }}
  <br>
  y : {{ y }}
  <br>
  x * y = {{ myFunction() }}
</template>

<style scoped>
  p {
    color: white;
    background-color: chocolate;
  }
</style>
