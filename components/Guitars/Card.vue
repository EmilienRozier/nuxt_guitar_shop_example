<template>
  <NuxtLink :to="'/guitars/' + id" class="flex w-[300px] min-w-[300px] m-5 justify-self-center">
    <div class="relative flex flex-col w-full overflow-hidden rounded-md transition bg-gray-300 hover:scale-105 hover:drop-shadow-sm">
      <div class="h-[300px] relative flex items-center overflow-hidden">
        <img :src="img" class="absolute left-0 w-full p-5 h-full object-contain">
      </div>
      <div class="bg-gray-100 p-5 flex h-full max-h-24">
        <h4><b>{{ titre }}</b></h4>
<!--        <h4>{{ details }}</h4>-->
      </div>
    </div>
  </NuxtLink>
</template>

<style scoped>
</style>

<script setup lang="ts">
defineProps<{
  img?: string
  titre?: string
  // details?: string
  id?: number
}>()
</script>