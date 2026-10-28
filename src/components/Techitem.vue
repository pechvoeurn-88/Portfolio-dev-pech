<script setup>
defineProps({
  short: String,
  name: String,
  active: Boolean,
})
</script>

<template>
  <div :class="['rounded-xl py-4 text-center text-ink', active ? 'bg-brand' : 'bg-white']">
    <p class="font-extrabold">{{ short }}</p>
    <p class="text-[10px] opacity-60">{{ name }}</p>
  </div>
</template>