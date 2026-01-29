<template>
  <div class="relative py-20 sm:pt-36 sm:pb-24">
    <BackgroundImage class="-top-36 -bottom-14" />
    <Container class="relative">
      <div class="mx-auto max-w-2xl lg:max-w-4xl lg:px-12">
        <h1 class="font-display text-5xl font-bold tracking-tighter text-blue-600 sm:text-7xl">
          <span class="sr-only">DeceptiConf - </span>O conferință de design pentru partea întunecată.
        </h1>
        <div class="mt-6 space-y-6 font-display text-2xl tracking-tight text-blue-900">
          <p>
            Noua generație de utilizatori web sunt versați și suspicioși. Știu cum să folosească
            instrumente de dezvoltare, pot detecta o înșelătoriu de la o depărtare mare și cu
            siguranță nu acceptă cecuri de la Western Union.
          </p>
          <p>
            La DeceptiConf veți învață despre cele mai noi modele întunecate în dezvoltare pentru a
            înșela chiar și vizitatorii mai inteligenți, și veți învață cum să le implementați fără
            a fi detectați.
          </p>
        </div>
        <Button href="#" class="mt-10 w-full sm:hidden">Obțineți bilete</Button>
        <dl
          class="mt-10 grid grid-cols-2 gap-x-10 gap-y-6 sm:mt-16 sm:gap-x-16 sm:gap-y-10 sm:text-center lg:auto-cols-auto lg:grid-flow-col lg:grid-cols-none lg:justify-start lg:text-left"
        >
          <div v-for="[name, value] in stats" :key="name">
            <dt class="font-mono text-sm text-blue-600">{{ name }}</dt>
            <dd class="mt-0.5 text-2xl font-semibold tracking-tight text-blue-900">
              {{ value }}
            </dd>
          </div>
        </dl>
      </div>
    </Container>
  </div>
</template>

<script setup>
import BackgroundImage from './BackgroundImage.vue'
import Button from './Button.vue'
import Container from './Container.vue'

const stats = [
  ['Vorbitori', '18'],
  ['Participanți', '2,091'],
  ['Loc', 'Staples Center'],
  ['Locație', 'Los Angeles'],
]
</script>
