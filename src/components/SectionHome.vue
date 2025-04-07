<script setup>
import HomeProfile from './HomeProfile.vue'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faLinkedinIn, faGithub } from '@fortawesome/free-brands-svg-icons'
import { profileData } from '@/constants/content'
</script>

<template>
  <section class="container mx-auto py-10 lg:py-16 px-4 md:px-8 lg:px-16 xl:px-32">
    <div class="lg:grid lg:grid-cols-2 items-center">
      <div>
        <h3 class="text-2xl lg:text-3xl font-semibold text-slate-100 mb-4">I am Romario</h3>
        <h1 class="text-4xl lg:text-6xl font-bold text-violet-400 mb-4">
          Software Developer
        </h1>
        <p class="text-lg lg:text-xl font-normal text-slate-100 mb-8">
          I propose ideas and solve problems by developing efficient,
          user-friendly and maintainable applications
        </p>
        <div class="flex flex-row items-center gap-4">
          <a
            href="https://drive.google.com/file/d/1MwKp9nMbgITAzfTaGjI6_PmrAiBKqeX6/view"
            class="transition-colors px-8 py-3 font-medium rounded-full border text-violet-500 border-violet-500 hover:text-white hover:bg-violet-500"
            target="_blank"
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
      <div class="mx-auto mt-12 lg:mt-0">
        <img
          class="w-full lg:ml-auto lg:w-[90%] rounded-3xl border-2 border-violet-950"
          src="../assets/images/home.jpg"
          alt=""
        />
      </div>
    </div>
    <HomeProfile :profile-data="profileData" />
  </section>
</template>
