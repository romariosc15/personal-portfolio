<script setup>
import NavigationBar from './components/Navigation/NavigationBar.vue'
import NavigationFooter from './components/Navigation/NavigationFooter.vue'
import NavigationScrollUp from './components/Navigation/NavigationScrollUp.vue'
import SectionHome from './components/SectionHome.vue'
import SectionPortfolio from './components/SectionPortfolio.vue'
import SectionResume from './components/SectionResume.vue'
import SectionContact from './components/SectionContact.vue'
</script>

<template>
  <div class="min-h-screen bg-[#0f0715]">
    <header>
      <NavigationBar />
    </header>

    <main>
      <SectionHome id="home" />
      <SectionPortfolio id="portfolio" />
      <SectionResume id="resume" />
      <SectionContact id="contact" />
    </main>
    <NavigationFooter />
    <NavigationScrollUp />
  </div>
</template>

<style scoped></style>
