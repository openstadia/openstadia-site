<script setup lang="ts">
import { onBeforeUnmount, onMounted, ref } from 'vue'

const words = ['Cloud Gaming', 'Cloud Workspace', 'Screen Sharing', 'Cloud Distribution']

let index = 0
const phrase = ref(words[index])
let intervalId: number

onMounted(() => {
  intervalId = setInterval(() => {
    index = (index + 1) % words.length
    phrase.value = words[index]
  }, 2000)
})

onBeforeUnmount(() => {
  clearInterval(intervalId)
})
</script>

<template>
  <div class="flex-1 flex items-center justify-center relative isolate px-4 py-14 lg:px-8">
    <div class="max-w-4xl">
      <div class="flex flex-col items-center text-center">
        <div class="flex items-center text-6xl">
          <img class="h-14 lg:h-24 w-auto mr-4 lg:mr-6" src="@/assets/openstadia.svg" alt="" />
          <span class="text-4xl lg:text-6xl font-title">OpenStadia</span>
        </div>

        <h1 class="mt-4 text-xl lg:text-2xl uppercase text-openstadia">{{ phrase }} Your Way</h1>

        <div class="flex flex-col">
          <div class="flex mt-12 lg:mt-18 sm:justify-center">
            <div
              class="relative rounded-full px-4 lg:px-6 py-2 text-sm leading-6 text-gray-600 ring-1 ring-gray-900/20"
            >
              🎉Release 0.2.0🎉
            </div>

            <a
              class="ml-4"
              href="https://github.com/openstadia/openstadia/releases/tag/v0.2.0-alpha"
            >
              <button
                type="button"
                class="flex items-center text-white bg-openstadia-500 hover:bg-openstadia-700 focus:ring-4 focus:ring-openstadia-300 font-medium rounded-lg text-sm px-5 py-2.5 focus:outline-none"
              >
                <span>Download Now</span>
                <svg
                  class="ml-2 w-4 h-4"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 16 18"
                >
                  <path
                    stroke="currentColor"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M8 1v11m0 0 4-4m-4 4L4 8m11 4v3a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2v-3"
                  />
                </svg>
              </button>
            </a>
          </div>

          <a class="mt-6" href="https://app.openstadia.com/">
            <button
              type="button"
              class="w-full flex justify-center items-center text-white bg-openstadia-500 hover:bg-openstadia-700 focus:ring-4 focus:ring-openstadia-300 font-medium rounded-lg text-sm px-5 py-2.5 focus:outline-none"
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
        </div>
      </div>
    </div>
  </div>
</template>
