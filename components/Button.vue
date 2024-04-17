<template>
  <NuxtLink :to="to" class="max-w-max bg-[#bf9500] px-10 py-3 uppercase" v-if="style === 0">
    <slot/>
  </NuxtLink>
  <NuxtLink :to="to" class="max-w-max border-solid border-[#bf9500] border-4 px-10 py-3 uppercase" v-if="style === 1">
    <slot/>
  </NuxtLink>
</template>

<script setup lang="ts">
defineProps<{
  to?: string
  style?: number
}>()
</script>