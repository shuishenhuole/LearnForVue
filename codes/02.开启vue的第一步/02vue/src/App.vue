<template>
<h1>{{ message }}</h1>
<button @click="incrment">increment</button>
</template>

<script setup lang="ts">
import { nextTick, ref, shallowRef } from 'vue'
   const message = ref(1)
  async function incrment(){
    message.value += 1
    // await nextTick()
   }
</script>

<style scoped>
    .red{
      color: red;
    }
</style>