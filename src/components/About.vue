<script setup>
import Education from './Education.vue'
import Techitem from './Techitem.vue'

const tools = [
  { short: 'JS', name: 'JavaScript', active: true },
  { short: 'LAR', name: 'Laravel' },
  { short: 'GIT', name: 'Git' },
  { short: 'PHP', name: 'PHP' },
  { short: 'TW', name: 'Tailwind' },
  { short: 'FIG', name: 'Figma' },
  { short: 'VUE', name: 'Vue' },
  { short: 'SQL', name: 'PostgreSQL' },
]
</script>

<template>
  <section id="about" class="bg-ink px-32 py-16 text-white">
    <p class="   font-bold uppercase">About me</p>
    <h2 class="mt-2 text-5xl font-extrabold">Developer, learner, and builder.</h2>
    <p class="mt-2 text-2xl w-200 text-white/60">I'm Pech, a web and mobile developer who likes turning real problems into simple, working apps.
       I learn by building, and I focus on clean interfaces and code that's easy to maintain.
    </p>

    <div class="mt-10 grid grid-cols-2 gap-16">
      <div>
        <p class="mb-3 text-xl font-bold uppercase">EDUCATION</p>
        <Education
          school="PSE Institute"
          course="IT / Web & Application Development"
          year="2nd Year • 2026"
        />
        <p class="mb-3 text-xl font-bold uppercase"></p>
        
      </div>
      
        

      <div>
        <p class="mb-3 text-xs font-bold uppercase">Tech stack</p>
        <div class="grid grid-cols-3 gap-3">
          <Techitem v-for="t in tools" :key="t.short" v-bind="t" />
        </div>
      </div>
    </div>
  </section>
</template>