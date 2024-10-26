<script setup>
const props = defineProps({
  tags: Array,
})
</script>
<template>
  <div class="flex flex-row gap-4 mb-8">
    <div
      v-for="(tag, index) in props.tags"
      :key="index"
      class="rounded-full bg-violet-900 text-white py-2 px-4"
    >
      {{ tag }}
    </div>
  </div>
</template>
