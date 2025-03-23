<script setup>
const props = defineProps({
  tags: Array,
})
</script>
<template>
  <div class="flex flex-row flex-wrap gap-4 mb-8">
    <div
      v-for="(tag, index) in props.tags"
      :key="index"
      class="rounded-full text-sm lg:text-base bg-violet-900 text-white py-1.5 lg:py-2 px-3 lg:px-4"
    >
      {{ tag }}
    </div>
  </div>
</template>
