<template>
  <header class="flex sticky top-0 z-50 items-center justify-between border-b border-black/10 bg-cream px-30 py-5">
    <a href="#" class="text-3xl font-extrabold">V.PECH</a>
    <nav class="flex gap-6  text-2xl">
      <a href="#home" 
          class="relative text-2xl font-medium text-ink
         after:absolute after:left-0 after:-bottom-1 after:h-[3px] after:w-0
         after:rounded-full after:bg-ink after:transition-all after:duration-200
         hover:after:w-full">Home</a>
      <a href="#work"
          class="relative text-2xl font-medium text-ink
         after:absolute after:left-0 after:-bottom-1 after:h-[3px] after:w-0
         after:rounded-full after:bg-ink after:transition-all after:duration-200
         hover:after:w-full">Work</a>
      <a href="#about" 
          class="relative text-2xl font-medium text-ink
         after:absolute after:left-0 after:-bottom-1 after:h-[3px] after:w-0
         after:rounded-full after:bg-ink after:transition-all after:duration-200
         hover:after:w-full">About</a>
      <a href="#contact"
        class="relative text-2xl font-medium text-ink
         after:absolute after:left-0 after:-bottom-1 after:h-[3px] after:w-0
         after:rounded-full after:bg-ink after:transition-all after:duration-200
         hover:after:w-full">Contact</a>
    </nav>
    <Button href="#Download-CV">Download CV</Button>
  </header>
</template>
<script setup>
import Button from './Button.vue'
</script>