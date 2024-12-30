<script setup>
import { experience, education } from '@/constants/content'
import ResumeCardContainer from './ResumeCardContainer.vue'
</script>

<template>
  <section class="container mx-auto py-16 px-16">
    <div class="text-center space-y-4 mb-12">
      <h2 class="text-4xl font-semibold text-violet-400">My Resume</h2>
      <p class="text-slate-100">PROFESSIONAL &amp; ACADEMIC BACKGROUND</p>
    </div>
    <div class="grid grid-cols-2 gap-16">
      <ResumeCardContainer title="Experience" :items="experience" />
      <ResumeCardContainer title="Education" :items="education" />
    </div>
  </section>
</template>
