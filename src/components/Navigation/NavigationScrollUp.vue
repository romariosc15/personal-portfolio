<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faArrowUp } from '@fortawesome/free-solid-svg-icons'

const scrollToTop = () => {
  window.scrollTo(0, 0)
}
</script>

<template>
  <button
    class="fixed bottom-12 right-16 text-violet-700 border-2 border-violet-700 rounded-full hover:bg-violet-700 hover:text-white transition-colors w-12 h-12 text-center content-center"
    @click="scrollToTop"
  >
    <FontAwesomeIcon class="w-6 h-6" :icon="faArrowUp" />
  </button>
</template>
