<template>
  <Header />
  <main class="flex-auto">
    <slot />
  </main>
  <Footer v-if="showFooter" />
</template>

<script setup>
import Footer from './Footer.vue'
import Header from './Header.vue'

defineProps({
  showFooter: {
    type: Boolean,
    default: true,
  },
})
</script>
