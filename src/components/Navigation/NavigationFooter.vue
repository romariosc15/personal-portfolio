<script setup>
import { navLinks } from '@/constants/content'
</script>

<template>
  <footer class="text-center py-4 lg:py-6 px-4 md:px-8 lg:px-16 xl:px-32 space-y-4">
    <div>
      <a href="#app">
        <img class="w-[75px] mx-auto" src="/src/assets/images/logo.png" alt="Portfolio logo">
      </a>
    </div>
    <nav>
      <ul class="text-white flex justify-center flex-row gap-8">
        <li v-for="(link, index) in navLinks" :key="index">
          <a
            class="transition-colors text-base font-semibold inline-block py-1 border-b-2 border-b-transparent hover:border-b-violet-700"
            :href="link.href"
            >{{ link.name }}</a
          >
        </li>
      </ul>
    </nav>
    <div>
      <p class="text-base font-light text-gray-500">
        Developed by Romario Sarmiento
      </p>
    </div>
  </footer>
</template>
