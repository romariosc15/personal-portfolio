<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faLink } from '@fortawesome/free-solid-svg-icons'
import ProjectTags from '../components/ProjectTags.vue'
import { projects } from '@/constants/content'
import { useAssets } from '@/composables/useAssets'
</script>

<template>
  <section class="bg-black">
    <div class="container mx-auto py-16 px-16">
      <div class="text-center space-y-4 mb-12">
        <h2 class="text-4xl font-semibold text-violet-400">My Portfolio</h2>
        <p class="text-slate-100">PERSONAL PROJECTS</p>
      </div>
      <div class="space-y-16">
        <div
          v-for="(project, index) in projects"
          :key="index"
          class="grid grid-cols-2 gap-12 px-12 py-16 rounded-xl border bg-[#15091d] border-violet-900"
        >
          <div>
            <span class="text-lg text-violet-500">{{ project.type }}</span>
            <h3 class="text-3xl font-medium text-white my-4">
              {{ project.title }}
            </h3>
            <p class="text-lg font-light text-white mb-8">
              {{ project.description }}
            </p>
            <ProjectTags :tags="project.tags" />
            <a
              :href="project.url"
              class="transition-colors text-white hover:text-violet-500"
              target="_blank"
            >
              Go to website
              <FontAwesomeIcon
                class="w-5 h-5 ml-1 align-middle"
                :icon="faLink"
              />
            </a>
          </div>
          <div>
            <img
              class="w-full rounded-xl border-[16px] border-[#10171c]"
              :src="useAssets(`/src/assets/images/projects/${project.image}`)"
              alt="Project image"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
