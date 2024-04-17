<template>
  <div class="flex">
    <NuxtLink to="/">
      <div class="h-10 flex items-center m-3">
        <img src="/img/charvel-logo.png" class="h-full">
      </div>
    </NuxtLink>
    <div class="flex w-full justify-center">
      <ul class="flex w-1/3 h-16 justify-between items-center">
        <li>
          <NuxtLink to="/guitars">guitars</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/basses">basses</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/accessories">accessories</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/customshop">customshop</NuxtLink>
        </li>
      </ul>
    </div>
  </div>
</template>
<script setup lang="ts">
</script>