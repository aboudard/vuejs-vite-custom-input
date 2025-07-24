<script setup>
import HelloWorld from './components/HelloWorld.vue'
import BaseInput from './components/BaseInput.vue'
import { ref } from "vue"

const data = ref({
  value: "empty",
  code: 54
})

</script>

<template>
  <div>
    {{ data }}
  </div>
  <HelloWorld msg="Vite + Vue" />
  <BaseInput v-model="data" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
