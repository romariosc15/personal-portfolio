<script setup>
const props = defineProps({
  title: String,
  items: Array,
})
</script>

<template>
  <div class="space-y-6 lg:space-y-8">
    <h2 class="text-3xl lg:text-4xl font-semibold text-slate-100">{{ props.title }}</h2>
    <div v-for="(item, index) in props.items" :key="index" class="space-y-4">
      <div class="bg-violet-700 rounded-3xl px-6 lg:px-10 py-4 lg:py-6 space-y-1">
        <span class="textl-lg lg:text-xl font-medium text-slate-100">{{
          item.period
        }}</span>
        <h3 class="text-2xl lg:text-3xl font-bold text-slate-100">
          {{ item.name }}
        </h3>
        <p class="text-base lg:text-lg font-light text-slate-100">
          {{ item.entity }}, {{ item.location }}
        </p>
      </div>
    </div>
  </div>
</template>
