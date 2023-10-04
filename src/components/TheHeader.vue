<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>

<template>
  <header class="sticky inset-x-0 top-0 z-50">
    <nav
      class="flex items-center justify-center lg:justify-between p-4 lg:px-8"
      aria-label="Global"
    >
      <RouterLink to="/" class="flex items-center lg:flex-1 lg:flex-shrink-0">
        <div class="flex items-center -m-1.5 p-1.5">
          <span class="font-title sr-only">OpenStadia</span>
          <img class="h-8 w-auto" src="@/assets/openstadia.svg" alt="" />
        </div>

        <span class="font-title ml-2 text-2xl">OpenStadia</span>
      </RouterLink>
    </nav>
  </header>
</template>
