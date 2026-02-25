<template>
  <div class="flex flex-col gap-0 pb-20">
    <Hero />
    <About />
    <MenuSection />
    <Reservation />
  </div>
</template>

<script setup>
import Hero from '@/components/Hero.vue'
import About from '@/components/About.vue'
import MenuSection from '@/components/MenuSection.vue'
import Reservation from '@/components/Reservation.vue'
</script>
