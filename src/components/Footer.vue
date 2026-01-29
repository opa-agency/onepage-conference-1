<template>
  <footer class="flex-none py-16">
    <Container class="flex flex-col items-center justify-between md:flex-row">
      <Logo class="h-12 w-auto text-slate-900" />
      <p class="mt-6 text-base text-slate-500 md:mt-0">
        Copyright &copy; {{ year }} DeceptiConf, LLC. All rights reserved.
      </p>
    </Container>
  </footer>
</template>

<script setup>
import { computed } from 'vue'
import Container from './Container.vue'
import Logo from './Logo.vue'

const year = computed(() => new Date().getFullYear())
</script>
