<script setup>
import { computed } from 'vue'
import { useWindowScroll } from '@vueuse/core'
import { navLinks } from '@/constants/content'

const { y } = useWindowScroll({ behavior: 'smooth' })

const staticTopBlockClass = computed(() => ({
  hidden: y.value <= 104,
  block: y.value > 104,
}))

const stickyNavbarClass = computed(() => ({
  'fixed top-0 bg-black shadow-xl shadow-violet-500/10': y.value > 104,
}))

</script>

<template>
  <div class="h-[104px]" :class="staticTopBlockClass"></div>
  <div class="w-full" :class="stickyNavbarClass">
    <div class="container mx-auto py-6 xl:py-8 px-4 md:px-8 lg:px-16 xl:px-32">
      <div class="flex flex-row items-center">
        <div class="mr-8">
          <a href="#app">
            <img class="w-[50px]" src="/src/assets/images/logo.png" alt="Portfolio logo">
          </a>
        </div>
        <div class="ml-auto md:ml-0 block md:hidden lg:block">
          <a
            class="transition-colors font-medium text-white hover:text-violet-500"
            href="mailto:romariosc15@outlook.com"
          >
            romariosc15@outlook.com
          </a>
        </div>
        <nav class="ml-auto hidden md:block">
          <ul class="text-white flex flex-row gap-12">
            <li v-for="(link, index) in navLinks" :key="index">
              <a
                class="transition-colors inline-block py-1 border-b-2 border-b-transparent hover:border-b-violet-700"
                :href="link.href"
                >{{ link.name }}</a
              >
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
