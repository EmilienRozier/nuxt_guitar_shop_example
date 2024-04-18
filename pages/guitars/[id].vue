<template>
  <NuxtLayout>
    <div class="grid grid-cols-2 w-3/4 mx-auto" v-for="g in guitars.data">
<!--      <guitars-card :key="g.id" :id="g.id" :titre="g.name" details="" :img="g.img"/>-->
      <div class="h-96 flex justify-center">
        <img :src="g.img" class="h-full w-auto">
      </div>
      <div>
        <h1>{{g.name}}</h1>
      </div>
    </div>
  </NuxtLayout>
</template>
<script setup lang="ts">

import {useRoute} from "vue-router";

definePageMeta({
  layout: 'custom',
})

let client = useSupabaseClient()
const route = useRoute()

let { data: guitars } = await useAsyncData('guitars', async () => client.from('guitars').select('*').eq('id', route.params.id))

</script>