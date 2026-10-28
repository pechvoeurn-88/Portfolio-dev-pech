<script setup>
import ProjectCard from './ProjectCard.vue'

const projects = [
  { number: '01', title: 'Smart Locker', stack: 'Laravel • PostgreSQL', description: 'Booking & locker management', variant: 'yellow' },
  { number: '02', title: 'Samai Map', stack: 'WordPress • Leaflet', description: 'Interactive venue map', variant: 'black' },
  { number: '03', title: 'Phone Shop', stack: 'Laravel • PHP', description: 'E-commerce platform', variant: 'white' },
]
</script>

<template>
  <section id="work" class="bg-cream px-24 py-12">
    <div class="flex items-start justify-between">
      <h2 class="text-5xl font-extrabold">Selected work</h2>
      <p>03 projects</p>
    </div>

    <div class="mt-10 space-y-4">
      <ProjectCard v-for="p in projects" :key="p.number" v-bind="p" />
    </div>
  </section>
</template>