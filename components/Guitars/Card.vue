<template>
  <NuxtLink :to="'/guitars/' + id" class="flex w-[300px] min-w-[300px] m-1 justify-self-center">
    <div class="relative flex flex-col w-full overflow-hidden bg-gray-300 rounded-md transition hover:scale-105">
      <div class="h-[300px] -rotate-90 relative flex items-center">
        <img :src="img" class="absolute left-0 w-[200%] p-5">
      </div>
      <div class="bg-gray-100 p-5">
        <h2>{{ titre }}</h2>
        <h3>{{ details }}</h3>
        <!--      <p>-->
        <!--        Featuring a sculpted shredder s cut heel and scalloped lower back bout for comfortable and unencumbered upper fret access, the Dinky® alder body is paired with a graphite-reinforced bolt-on caramelized maple neck for rock-solid stability. The baked neck has a silky-smooth hand-rubbed satin urethane finish on the back for sublime playability, Luminlay® side dots to guide your way along the fretboard on dark stages and a heel-mount truss rod adjustment wheel for quick and painless neck relief tweaks. Designed for high-speed playing, its 12"-16" compound radius ebony fingerboard features comfortable rolled edges, 24 jumbo frets, pearloid dot inlays and Graph Tech® TUSQ® XL nut.-->
        <!--      </p>-->
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