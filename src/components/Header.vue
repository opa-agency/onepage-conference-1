<template>
  <header class="relative z-50 flex-none lg:pt-11">
    <Container class="flex flex-wrap items-center justify-center sm:justify-between lg:flex-nowrap">
      <div class="mt-10 lg:mt-0 lg:grow lg:basis-0">
        <Logo class="h-12 w-auto text-slate-900" />
      </div>
      <div
        class="order-first -mx-4 flex flex-auto basis-full overflow-x-auto border-b border-blue-600/10 py-4 font-mono text-sm whitespace-nowrap text-blue-600 sm:-mx-6 lg:order-0 lg:mx-0 lg:basis-auto lg:border-0 lg:py-0"
      >
        <div class="mx-auto flex items-center gap-4 px-4">
          <p>
            <time datetime="2022-04-04">04</time>-<time datetime="2022-04-06">06 aprilie, 2022</time>
          </p>
          <DiamondIcon class="h-1.5 w-1.5 overflow-visible fill-current stroke-current" />
          <p>Los Angeles, CA</p>
        </div>
      </div>
      <div class="hidden sm:mt-10 sm:flex lg:mt-0 lg:grow lg:basis-0 lg:justify-end">
        <Button href="#">Obțineți bilete</Button>
      </div>
    </Container>
  </header>
</template>

<script setup>
import Button from './Button.vue'
import Container from './Container.vue'
import DiamondIcon from './DiamondIcon.vue'
import Logo from './Logo.vue'
</script>
