<script setup>
import Button from './Button.vue'
</script>

<template>
  <section id="home" class="flex items-center h-180  justify-between bg-cream px-32 ">
    <div class=" mb-50 mt-40">
      <p class="text-xl font-bold uppercase text-black/60">WEB + MOBILE DEVELOPER</p>
      <h1 class="mt-6 text-8xl font-extrabold">Hi, I'm Pech.</h1>
      <p class="mt-6 text-4xl max-w-160 font-bold">I build fast, reliable web and mobile apps, from idea to launch.</p>
      <p class="mt-3 text-2xl text-black/60">Full-Stack focused • Web • Mobile Application</p>
      <div class="mt-8 flex gap-3">
        <Button href="#work">View work</Button>
        <Button variant="yellow" href="#contact">Contact</Button>
      </div>
    </div>
    <div class="size-96  mb-50 mr-30 w-150">

     <img src="../assets/images/me.jpeg" alt="me" class="w-150 rounded-full" />
    </div>
  </section>
</template> 