<template>
  <section id="newsletter" aria-label="Newsletter">
    <Container>
      <div
        class="relative -mx-4 overflow-hidden bg-indigo-50 px-4 py-20 sm:-mx-6 sm:px-6 md:mx-0 md:rounded-5xl md:px-16 xl:px-24 xl:py-36"
      >
        <img
          class="absolute top-0 left-1/2 translate-x-[-10%] translate-y-[-45%] lg:translate-x-[-32%]"
          :src="backgroundImage"
          alt=""
          width="919"
          height="1351"
        />
        <div
          class="relative mx-auto grid max-w-2xl grid-cols-1 gap-x-32 gap-y-14 xl:max-w-none xl:grid-cols-2"
        >
          <div>
            <p class="font-display text-4xl font-medium tracking-tighter text-blue-900 sm:text-5xl">
              Rămâneți la curent
            </p>
            <p class="mt-4 text-lg tracking-tight text-blue-900">
              Obțineți actualizări la toate evenimentele noastre și fiți printre primii notificați când biletele se pun în vânzare.
            </p>
          </div>
          <form>
            <h3 class="text-lg font-semibold tracking-tight text-blue-900">
              Abonați-vă la newsletter-ul nostru <span aria-hidden="true">&darr;</span>
            </h3>
            <div
              class="mt-5 flex rounded-3xl bg-white py-2.5 pr-2.5 shadow-xl shadow-blue-900/5 focus-within:ring-2 focus-within:ring-blue-900"
            >
              <input
                type="email"
                required
                placeholder="Adresă de email"
                aria-label="Adresă de email"
                class="-my-2.5 flex-auto bg-transparent pr-2.5 pl-6 text-base text-slate-900 placeholder:text-slate-400 focus:outline-hidden"
              />
              <Button type="submit" class="flex-none">
                <span class="sr-only sm:not-sr-only">Abonați-vă azi</span>
                <span class="sm:hidden">
                  <svg aria-hidden="true" viewBox="0 0 24 24" class="h-6 w-6">
                    <path
                      d="m14 7 5 5-5 5M19 12H5"
                      fill="none"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </span>
              </Button>
            </div>
          </form>
        </div>
      </div>
    </Container>
  </section>
</template>

<script setup>
import Button from './Button.vue'
import Container from './Container.vue'
import backgroundImage from '../images/background-newsletter.jpg'
</script>
