<script setup>
  import IconPlus from './components/icons/IconPlus.vue'
  import IconMinus from './components/icons/IconMinus.vue'
  import {ref} from 'vue'
  const num = ref(0)

</script>

<template>
    <label for="">count : {{num}}</label>
    <br>
    <button class="Plus" @click="num++"><IconPlus /></button>
    <button class="Minus" @click="num--"><IconMinus /></button>
</template>

<style scoped>
  .Plus {
    border-radius: 10%;
    background-color: aquamarine;
  }


  .Minus {
    border-radius: 10%;
    background-color: palevioletred;
  }

  button {
    margin-top: 1ch;
    margin-right: 2ch;
  }
</style>


<!-- <script setup>
import { ref } from 'vue'
const count = ref(0)
</script>

<template>
  <button @click="count++">Count is: {{ count }}</button>
</template>

<style scoped>
button {
  font-weight: bold;
}
</style> -->