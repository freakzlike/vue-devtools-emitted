<template>
  <BaseButton v-bind="$attrs" @click="emit('click')" />
</template>

<script setup lang="ts">
import BaseButton from './BaseButton.vue'

const emit = defineEmits<{
  (e: 'click'): void
}>()
</script>