<template>
  <NuxtLink :to="'/guitars/' + id" class="flex w-[300px] min-w-[300px] m-5 justify-self-center">
    <div class="relative flex flex-col w-full overflow-hidden bg-gray-300 rounded-md transition hover:scale-105">
      <div class="h-[300px] -rotate-90 relative flex items-center">
        <img :src="img" class="absolute left-0 w-[200%] p-5">
      </div>
      <div class="bg-gray-100 p-5">
        <h4><b>{{ titre }}</b></h4>
        <h4>{{ details }}</h4>
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
  details?: string
  id?: number
}>()
</script>