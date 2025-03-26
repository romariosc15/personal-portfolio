<script setup>
import { experience, education } from '@/constants/content'
import ResumeCardContainer from './ResumeCardContainer.vue'
</script>

<template>
  <section class="container mx-auto py-10 lg:py-16 px-4 md:px-8 lg:px-16 xl:px-36 scroll-mt-[60px]">
    <div class="text-center space-y-4 mb-12">
      <h2 class="text-4xl font-semibold text-violet-400">My Resume</h2>
      <p class="text-slate-100">PROFESSIONAL &amp; ACADEMIC BACKGROUND</p>
    </div>
    <div class="md:grid md:grid-cols-2 md:gap-8 lg:gap-16 space-y-8 md:space-y-0">
      <ResumeCardContainer title="Experience" :items="experience" />
      <ResumeCardContainer title="Education" :items="education" />
    </div>
  </section>
</template>
