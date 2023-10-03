<script setup lang="ts">
import TheJoin from '@/components/TheJoin.vue'
</script>

<template>
  <div class="flex-1 flex items-center justify-center relative isolate px-4 py-14 lg:px-8">
    <div class="max-w-4xl">
      <div class="flex flex-col items-center text-center">
        <div class="flex items-center text-6xl">
          <img class="h-14 lg:h-24 w-auto mr-4 lg:mr-6" src="@/assets/openstadia.svg" alt="" />
          <span class="text-4xl lg:text-6xl">OpenStadia</span>
        </div>

        <h1 class="mt-4 text-xl lg:text-2xl uppercase text-openstadia">Cloud Gaming Your Way</h1>

        <div class="flex mt-8 lg:mt-24 sm:justify-center">
          <div
            class="relative rounded-full px-4 lg:px-6 py-2 text-sm leading-6 text-gray-600 ring-1 ring-gray-900/10 hover:ring-gray-900/20"
          >
            Announcement Coming Soon
          </div>
        </div>

        <div class="mt-8 lg:w-full">
          <TheJoin></TheJoin>
        </div>
      </div>
    </div>
  </div>
</template>
