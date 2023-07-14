<script setup>
import Child from '@/components/Child.vue'
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  ++count.value
}

const decrement = () => {
  --count.value
}
</script>

<template>
  <div class="container">
    <h1>Emits in Vue3</h1>
    <Child @inc="increment" @dec="decrement" />
    <h2>{{ count }}</h2>
  </div>
</template>

<style></style>
