<script setup>
import NavigationBar from './components/Navigation/NavigationBar.vue'
import NavigationFooter from './components/Navigation/NavigationFooter.vue'
import SectionHome from './components/SectionHome.vue'
import SectionPortfolio from './components/SectionPortfolio.vue'
</script>

<template>
  <div class="min-h-screen bg-[#0f0715]">
    <header>
      <NavigationBar />
    </header>

    <main>
      <SectionHome />
      <SectionPortfolio />
    </main>
    <NavigationFooter />
  </div>
</template>

<style scoped></style>
