<script setup>
import { ref } from 'vue'

const num = ref(2)
function clickMe() {
  num.value += 15
}
</script>

<template>
  {{ num }}

  <button type="button" v-on:click="clickMe">點我</button>
</template>
