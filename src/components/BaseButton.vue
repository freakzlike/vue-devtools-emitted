<template>
  <button @click="emit('click')">
    {{ label }}
  </button>
</template>

<script setup lang="ts">
defineProps<{
  label?: string
}>()

const emit = defineEmits<{
  (e: 'click'): void
}>()
</script>
