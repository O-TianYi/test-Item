<template>
  <div>
    <span>哈哈哈{{ res.msg }}</span>
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive } from 'vue'
import axios from '../utils/axios'

export default defineComponent({
  setup() {
    let result = reactive({})
    axios('/user/')
      .then((res) => {
        result = res
      })
      .catch((error) => {
        console.log(error)
      })
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
