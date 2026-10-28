<script setup>
defineProps({
  school: String,
  course: String,
  year: String,
  currentStudy: String,
  doOn: String,
  lookFor:String,
})
</script>

<template>
  <div class="rounded-2xl bg-white p-6 text-ink">
    <h3 class="text-3xl font-extrabold">{{ school }}</h3>
    <p class="mt-2 text-xl text-black/70">{{ course }}</p>
    <p class="mt-1 text-xl text-black/60">{{ year }}</p>
  </div>
  <div class="rounded-2xl bg-white p-6 text-ink" >
    <div >
      <h2>BoK</h2>
    </div>
    <div>
      <h3 class="text-3xl font-extrabold">{{ currentStudy }}</h3>
      <p class="mt-2 text-xl text-black/70">{{ doOn }}</p>
    </div>
    
  </div>
</template>