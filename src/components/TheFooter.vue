<script setup lang="ts">
import IconGithub from '@/components/icons/IconGithub.vue'
</script>

<template>
  <footer>
    <div class="p-2 lg:p-4 lg:px-6">
      <div class="flex pt-2 lg:pt-4 justify-between border-t border-gray-400">
        <div class="flex items-baseline">
          <div class="font-title lg:text-s">OpenStadia</div>
          <a href="https://utkin.tech/" class="font-utkin ml-2 text-xs text-gray-600"
            >by utkin.tech</a
          >
        </div>

        <div class="flex">
          <a class="text-gray-600 hover:text-gray-400" href="https://github.com/openstadia">
            <span class="sr-only">GitHub</span>
            <IconGithub class="h-6 w-6"></IconGithub>
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>
