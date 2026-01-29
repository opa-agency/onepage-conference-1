<template>
  <div class="flex min-h-full bg-white antialiased font-sans">
    <div class="flex w-full flex-col">
      <Layout>
        <Hero />
        <Speakers />
        <Schedule />
        <Sponsors />
        <Newsletter />
      </Layout>
    </div>
  </div>
</template>

<script setup>
import Hero from './components/Hero.vue'
import Layout from './components/Layout.vue'
import Newsletter from './components/Newsletter.vue'
import Schedule from './components/Schedule.vue'
import Speakers from './components/Speakers.vue'
import Sponsors from './components/Sponsors.vue'
</script>
