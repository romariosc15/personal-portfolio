<script setup>
const props = defineProps({
  profileData: Array,
})
</script>
<template>
    <div class="grid grid-cols-2 lg:flex lg:flex-row lg:flex-wrap lg:justify-between gap-y-4 lg:gap-y-0 pt-12 lg:pt-24">
        <div
            v-for="(data, index) in props.profileData"
            :key="index"
            class="flex flex-row justify-center lg:justify-normal items-center gap-4"
        >
            <span class="text-5xl md:text-6xl font-bold text-slate-100">{{ data.number }}</span>
            <p class="text-slate-100 text-sm md:text-base">
            {{ data.topText }} <br />
            {{ data.bottomText }}
            </p>
        </div>
    </div>
</template>
