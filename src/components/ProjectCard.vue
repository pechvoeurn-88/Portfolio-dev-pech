<script setup>
defineProps({
  number: String,
  title: String,
  stack: String,
  description: String,
  variant: { type: String, default: 'white' },
})

const variants = {
  yellow: 'bg-brand text-ink',
  black: 'bg-ink text-white',
  white: 'bg-white text-ink',
}
</script>

<template>
  <div :class="['flex gap-6 rounded-3xl p-6', variants[variant]]">
    <span class="text-xs font-bold">{{ number }}</span>

    <div class="grid h-44 w-80 place-items-center rounded-xl bg-cream font-bold text-ink">
      PROJECT
    </div>

    <div>
      <h3 class="text-2xl font-extrabold uppercase">{{ title }}</h3>
      <p class="text-sm opacity-70">{{ stack }}</p>
      <p class="mt-1">{{ description }}</p>
    </div>

    <span class="ml-auto self-center text-2xl">→</span>
  </div>
</template>