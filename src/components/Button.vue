<script setup>
defineProps({
  variant: { type: String, default: 'dark' },
  href: String,
})

const styles = {
  dark: 'bg-ink text-white  ',
  yellow: 'bg-brand text-white hover:bg-ink hover:text-white',
  white: 'bg-white text-ink hover:bg-ink hover:text-white',
}
</script>

<template>
  <a :href="href" :class="['inline-block rounded-full px-8 py-3 text-sm font-bold uppercase', styles[variant]]">
    <slot />
  </a>
</template>