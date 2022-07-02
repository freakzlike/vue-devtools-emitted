<template>
  <main>
    <PassAttrsButton
      label="Button with pass-through of events"
      @click="onPassAttrsClick"
    />
    <div>
      Logs events of BaseButton and not PassAttrsButton
    </div>

    <hr />

    <EmitButton
      label="Button with normal emit"
      @click="onEmitClick"
    />
    <div>
      Logs events of BaseButton and EmitButton
    </div>
  </main>
</template>

<script setup lang="ts">
import PassAttrsButton from './components/PassAttrsButton.vue'
import EmitButton from './components/EmitButton.vue'

const onPassAttrsClick = () => {
  console.log('Clicked PassAttrsButton')
}

const onEmitClick = () => {
  console.log('Clicked EmitButton')
}
</script>
