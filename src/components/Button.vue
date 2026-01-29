<template>
  <component
    :is="isLink ? 'a' : 'button'"
    :href="isLink ? href : undefined"
    :type="isLink ? undefined : type"
    :class="[baseClasses, $attrs.class]"
    v-bind="$attrs"
  >
    <slot />
  </component>
</template>

<script setup>
import { computed } from 'vue'

const props = defineProps({
  href: {
    type: String,
    default: undefined,
  },
  type: {
    type: String,
    default: 'button',
  },
})

const baseClasses =
  'inline-flex justify-center rounded-2xl bg-blue-600 p-4 text-base font-semibold text-white hover:bg-blue-500 focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-blue-500 active:text-white/70'

const isLink = computed(() => typeof props.href === 'string' && props.href.length > 0)
</script>
