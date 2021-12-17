<template>
  <div>
    <span>哈哈哈{{ res.msg }}</span>
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive } from 'vue'

export default defineComponent({
  setup() {
    const result = reactive({})
    return {
      result
    }
  }
})
</script>

<style lang="less" scoped>
div {
  background-color: red;
  span {
    color: white;
  }
}
</style>
