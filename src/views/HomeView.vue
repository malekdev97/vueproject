<script setup>
import TheWelcome from '../components/TheWelcome.vue'
import { ref } from 'vue'

const name = ref();

name.value = 'Vue 3'
window.nameRef = name; // expose variable to global scope whcih is a browser 
</script>

<template>
  <main>
    <h1>{{ name }}</h1>
  </main>
</template>
