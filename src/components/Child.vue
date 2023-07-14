<script setup>
const emit = defineEmits(['inc', 'dec'])
const inc = () => {
  emit('inc')
}
const dec = () => {
  emit('dec')
}
</script>

<template>
  <div class="row my-4">
    <div class="d-flex gap-3">
      <button @click="inc" class="btn btn-primary">Increment</button>
      <button @click="dec" class="btn btn-secondary">Decrement</button>
    </div>
  </div>
</template>

<style scoped></style>
