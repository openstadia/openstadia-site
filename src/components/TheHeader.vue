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

      <a href="https://app.openstadia.com/">
        <button
          type="button"
          class="hidden lg:flex items-center text-white bg-openstadia-500 hover:bg-openstadia-700 focus:ring-4 focus:focus:ring-openstadia-300 font-medium rounded-lg text-sm px-5 py-2.5 focus:outline-none"
        >
          <span>Try App</span>
          <svg
            class="ml-2 w-4 h-4"
            aria-hidden="true"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 18 18"
          >
            <path
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 11v4.833A1.166 1.166 0 0 1 13.833 17H2.167A1.167 1.167 0 0 1 1 15.833V4.167A1.166 1.166 0 0 1 2.167 3h4.618m4.447-2H17v5.768M9.111 8.889l7.778-7.778"
            />
          </svg>
        </button>
      </a>
    </nav>
  </header>
</template>
