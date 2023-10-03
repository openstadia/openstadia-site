<script setup lang="ts">
import { RouterView } from 'vue-router'
import TheHeader from '@/components/TheHeader.vue'
import TheFooter from '@/components/TheFooter.vue'
</script>

<template>
  <div class="h-screen bg-white flex flex-col">
    <TheHeader></TheHeader>

    <RouterView />

    <TheFooter></TheFooter>
  </div>
</template>
