<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faLinkedinIn, faGithub } from '@fortawesome/free-brands-svg-icons'
</script>

<template>
  <section class="container mx-auto py-16 px-16">
    <div class="grid grid-cols-2 items-center">
      <div>
        <h3 class="text-3xl font-semibold text-slate-100 mb-4">I am Romario</h3>
        <h1 class="text-6xl font-bold text-violet-400 mb-4">
          Full Stack Developer
        </h1>
        <p class="text-xl font-normal text-slate-100 mb-8">
          I suggest ideas and solve problems by developing efficient,
          user-friendly and maintainable applications over time
        </p>
        <div class="flex flex-row items-center gap-4">
          <a
            href="https://drive.google.com/file/d/1MwKp9nMbgITAzfTaGjI6_PmrAiBKqeX6/view"
            class="transition-colors px-8 py-3 font-medium rounded-full border text-violet-500 border-violet-500 hover:text-white hover:bg-violet-500"
          >
            Download CV
          </a>
          <a
            class="transition-colors flex items-center justify-center rounded-full border text-violet-500 border-violet-500 hover:text-white hover:bg-violet-500 p-2"
            href="https://www.linkedin.com/in/romariosarmiento/"
            target="_blank"
          >
            <FontAwesomeIcon class="w-5 h-5" :icon="faLinkedinIn" />
          </a>
          <a
            class="transition-colors flex items-center justify-center rounded-full border text-violet-500 border-violet-500 hover:text-white hover:bg-violet-500 p-2"
            href="https://github.com/romariosc15"
            target="_blank"
          >
            <FontAwesomeIcon class="w-5 h-5" :icon="faGithub" />
          </a>
        </div>
      </div>
      <div class="mx-auto">
        <img
          class="w-[600px] rounded-3xl border-2 border-violet-950"
          src="../assets/images/home.jpg"
          alt=""
        />
      </div>
    </div>
    <div class="flex flex-row justify-between pt-24">
      <div class="flex flex-row items-center gap-4">
        <span class="text-6xl font-bold text-slate-100">+5</span>
        <p class="text-slate-100">
          Years of <br />
          Experience
        </p>
      </div>
      <div class="flex flex-row items-center gap-4">
        <span class="text-6xl font-bold text-slate-100">3</span>
        <p class="text-slate-100">
          Certifications <br />
          Obtained
        </p>
      </div>
      <div class="flex flex-row items-center gap-4">
        <span class="text-6xl font-bold text-slate-100">2</span>
        <p class="text-slate-100">
          Languages <br />
          Proficiency
        </p>
      </div>
      <div class="flex flex-row items-center gap-4">
        <span class="text-6xl font-bold text-slate-100">F+B</span>
        <p class="text-slate-100">
          Frontend &amp; Backend <br />
          Development
        </p>
      </div>
    </div>
  </section>
</template>
