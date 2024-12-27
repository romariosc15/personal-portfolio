<script setup>
import { experience, education } from '@/constants/content'
</script>

<template>
  <section class="container mx-auto py-16 px-16">
    <div class="text-center space-y-4 mb-12">
      <h2 class="text-4xl font-semibold text-violet-400">My Resume</h2>
      <p class="text-slate-100">PROFESSIONAL &amp; ACADEMIC BACKGROUND</p>
    </div>
    <div class="grid grid-cols-2 gap-16">
      <div class="space-y-8">
        <h2 class="text-4xl font-semibold text-slate-100">Experience</h2>
        <div v-for="(job, index) in experience" :key="index" class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100">{{
              job.period
            }}</span>
            <h3 class="text-3xl font-bold text-slate-100">{{ job.role }}</h3>
            <p class="text-lg font-light text-slate-100">
              {{ job.company }}, {{ job.location }}
            </p>
          </div>
        </div>
      </div>
      <div class="space-y-8">
        <h2 class="text-4xl font-semibold text-slate-100">Education</h2>
        <div v-for="(study, index) in education" :key="index" class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100">{{
              study.period
            }}</span>
            <h3 class="text-3xl font-bold text-slate-100">
              {{ study.specialization }}
            </h3>
            <p class="text-lg font-light text-slate-100">
              {{ study.institute }}, {{ study.location }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
