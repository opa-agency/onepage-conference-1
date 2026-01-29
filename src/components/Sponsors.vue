<template>
  <section id="sponsors" aria-label="Sponsors" class="py-20 sm:py-32">
    <Container>
      <h2 class="mx-auto max-w-2xl text-center font-display text-4xl font-medium tracking-tighter text-blue-900 sm:text-5xl">
        Sponsorshipuri actuale pentru atelierele și vorbitorii noștri.
      </h2>
      <div
        class="mx-auto mt-20 grid max-w-max grid-cols-1 place-content-center gap-x-32 gap-y-12 sm:grid-cols-3 md:gap-x-16 lg:gap-x-32"
      >
        <div v-for="sponsor in sponsors" :key="sponsor.name" class="flex items-center justify-center">
          <img :src="sponsor.logo" :alt="sponsor.name" />
        </div>
      </div>
    </Container>
  </section>
</template>

<script setup>
import Container from './Container.vue'
import logoLaravel from '../images/logos/laravel.svg'
import logoMirage from '../images/logos/mirage.svg'
import logoStatamic from '../images/logos/statamic.svg'
import logoStaticKit from '../images/logos/statickit.svg'
import logoTransistor from '../images/logos/transistor.svg'
import logoTuple from '../images/logos/tuple.svg'

const sponsors = [
  { name: 'Transistor', logo: logoTransistor },
  { name: 'Tuple', logo: logoTuple },
  { name: 'StaticKit', logo: logoStaticKit },
  { name: 'Mirage', logo: logoMirage },
  { name: 'Laravel', logo: logoLaravel },
  { name: 'Statamic', logo: logoStatamic },
]
</script>
