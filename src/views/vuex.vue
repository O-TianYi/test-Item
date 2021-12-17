<template>
  <div>{{ msg }}</div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  setup() {
    const msg = ref('')
    msg.value = 'hello world'
    return {
      msg
    }
  }
})
</script>
