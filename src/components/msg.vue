<script setup>
defineProps({
    msg_str: {
    type: String,
    required: true
  }
})
</script>

<template>
      <h1>123 : {{ msg_str }}</h1>
</template>

