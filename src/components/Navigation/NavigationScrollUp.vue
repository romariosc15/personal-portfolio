<script setup>
import { computed } from 'vue'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faArrowUp } from '@fortawesome/free-solid-svg-icons'
import { useWindowScroll } from '@vueuse/core'

const { y } = useWindowScroll({ behavior: 'smooth' })

const scrollToTop = () => {
  y.value = 0
}

const isHidden = computed(() => {
  return y.value === 0 ? 'hidden' : 'block'}
)
</script>

<template>
  <div class="hidden xl:block">
    <button
      class="fixed bottom-12 right-14 text-violet-700 border-2 border-violet-700 rounded-full hover:bg-violet-700 hover:text-white transition-colors w-12 h-12"
      :class="isHidden"
      @click="scrollToTop"
    >
      <FontAwesomeIcon class="w-6 h-6 align-middle" :icon="faArrowUp" />
    </button>
  </div>
</template>
