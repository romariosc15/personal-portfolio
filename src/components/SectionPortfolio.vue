<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faLink } from '@fortawesome/free-solid-svg-icons'
import ProjectTags from '../components/ProjectTags.vue'
</script>

<template>
  <section class="bg-black">
    <div class="container mx-auto py-16 px-16">
      <div class="text-center space-y-4 mb-12">
        <h2 class="text-4xl font-semibold text-violet-400">My Portfolio</h2>
        <p class="text-slate-100">PERSONAL PROJECTS</p>
      </div>
      <div class="">
        <div
          class="grid grid-cols-2 gap-12 px-12 py-16 rounded-xl border bg-[#15091d] border-violet-900"
        >
          <div>
            <span class="text-lg text-violet-500">Web Application</span>
            <h3 class="text-3xl font-medium text-white my-4">Enjoyb</h3>
            <p class="text-lg font-light text-white mb-8">
              Aplicación desarrollada en Next.js e integrada con Contentful API
              para gestionar y publicar oportunidades de trabajo.
            </p>
            <ProjectTags
              :tags="['React', 'Next.js', 'Contentful', 'Tailwind']"
            />
            <a
              href="https://enjoyb.vercel.app/"
              class="transition-colors text-white hover:text-violet-500"
              target="_blank"
            >
              Visitar aplicación web
              <FontAwesomeIcon
                class="w-5 h-5 ml-1 align-middle"
                :icon="faLink"
              />
            </a>
          </div>
          <div>
            <img
              class="w-full rounded-xl border-[16px] border-[#10171c]"
              src="../assets/images/projects/enjoyb.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
