<template>
  <h1>{{result}}</h1>
</template>

<script lang="ts">
import { defineComponent } from "vue"
export default defineComponent({
  setup() {
    return new Promise(resolve => {
      setTimeout(() => {
        return resolve({
          result: "我是异步的"
        })
      }, 3000)
    })
  }
})
</script>