<template>
  <div class="w-full h-[70vh] bg-guitar relative">
    <div class=" flex flex-col m-3 absolute bottom-0 right-0 text-white items-end">
      <h2 class="">
        explore 2024 new release
      </h2>
      <Button to="/guitars/new" :style="1">
        view now
      </Button>
    </div>
  </div>

  <guitars-wrapper>
    <guitars-card id="1" titre="PRO-MOD DK24 HH 2PT EB" details="2962411303 / GLOSS BLACK" img="/img/guitars/pro-mod/pro-mod-1.png"/>
    <guitars-card id="1" titre="PRO-MOD DK24 HH 2PT EB" details="2962411303 / GLOSS BLACK" img="/img/guitars/pro-mod/pro-mod-1.png"/>
    <guitars-card id="1" titre="PRO-MOD DK24 HH 2PT EB" details="2962411303 / GLOSS BLACK" img="/img/guitars/pro-mod/pro-mod-1.png"/>
    <guitars-card id="1" titre="PRO-MOD DK24 HH 2PT EB" details="2962411303 / GLOSS BLACK" img="/img/guitars/pro-mod/pro-mod-1.png"/>
    <guitars-card id="1" titre="PRO-MOD DK24 HH 2PT EB" details="2962411303 / GLOSS BLACK" img="/img/guitars/pro-mod/pro-mod-1.png"/>
  </guitars-wrapper>

  <Feature/>

</template>

<script setup lang="ts">
</script>

<style scoped>
.bg-guitar {
  background: url("/img/charvel-new-releases-bg.jpg") center 0;
}
</style>