<template>
  <div>
    <guitars-wrapper>
      <guitars-largest-card />
      <guitars-card v-for="g in guitars.data" :key="g.id" :id="g.id" :titre="g.name" details="" :img="g.img"/>
    </guitars-wrapper>
  </div>
</template>

<script setup lang="ts">
let client = useSupabaseClient()

let { data: guitars } = await useAsyncData('guitars', async () => client.from('guitars').select('*'))

// console.log(guitars.value)

</script>