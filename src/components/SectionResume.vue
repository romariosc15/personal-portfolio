<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faSuitcase, faGraduationCap } from '@fortawesome/free-solid-svg-icons'
</script>

<template>
  <section class="container mx-auto py-16 px-16">
    <div class="text-center space-y-4 mb-12">
      <h2 class="text-4xl font-semibold text-violet-400">My Resume</h2>
      <p class="text-slate-100">PROFESSIONAL &amp; ACADEMIC BACKGROUND</p>
    </div>
    <div class="grid grid-cols-2 gap-16">
      <div class="space-y-8">
        <h2 class="text-4xl font-semibold text-slate-100">
          <FontAwesomeIcon class="align-middle w-7 mr-2" :icon="faSuitcase" />
          Experience
        </h2>
        <div class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100"
              >2024 May. - Present</span
            >
            <h3 class="text-3xl font-bold text-slate-100">Web UI Developer</h3>
            <p class="text-lg font-light text-slate-100">Globant, Remote</p>
          </div>
        </div>
        <div class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100"
              >2022 Dec. - 2024 Jan.</span
            >
            <h3 class="text-3xl font-bold text-slate-100">Software Engineer</h3>
            <p class="text-lg font-light text-slate-100">Intive, Remote</p>
          </div>
        </div>
        <div class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100"
              >2021 Nov. - 2022 Nov.</span
            >
            <h3 class="text-3xl font-bold text-slate-100">Web UI Developer</h3>
            <p class="text-lg font-light text-slate-100">Globant, Remote</p>
          </div>
        </div>
        <div class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100"
              >2020 Sep. - 2021 Oct.</span
            >
            <h3 class="text-3xl font-bold text-slate-100">Software Engineer</h3>
            <p class="text-lg font-light text-slate-100">Oktana, Remote</p>
          </div>
        </div>
        <div class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100"
              >2019 Sep. - 2020 Aug.</span
            >
            <h3 class="text-3xl font-bold text-slate-100">
              Full Stack Web Developer
            </h3>
            <p class="text-lg font-light text-slate-100">Innovahora, Ilo</p>
          </div>
        </div>
      </div>
      <div class="space-y-8">
        <h2 class="text-4xl font-semibold text-slate-100">
          <FontAwesomeIcon
            class="align-middle w-10 mr-2"
            :icon="faGraduationCap"
          />
          Education
        </h2>
        <div class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100"
              >2020 Jul. - 2020 Dec.</span
            >
            <h3 class="text-3xl font-bold text-slate-100">
              Full Stack Development Course
            </h3>
            <p class="text-lg font-light text-slate-100">TECSUP, Peru</p>
          </div>
        </div>
        <div class="space-y-4">
          <div class="bg-violet-600 rounded-3xl px-10 py-6 space-y-1">
            <span class="text-xl font-medium text-slate-100"
              >2015 Mar. - 2019 Dec.</span
            >
            <h3 class="text-3xl font-bold text-slate-100">
              Systems Engineering and Informatics
            </h3>
            <p class="text-lg font-light text-slate-100">
              Universidad Nacional de Moquegua, Peru
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
