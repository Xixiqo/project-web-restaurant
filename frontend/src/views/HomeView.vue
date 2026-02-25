<template>
  <div>
    <Hero />
    <MenuSection />
    
    <!-- About Section -->
    <section id="about" class="py-24 bg-[var(--color-primary-light)]">
      <div class="max-w-[1280px] mx-auto px-6 text-center">
        <h2 class="text-sm font-serif italic text-[var(--color-accent-gold)] tracking-[0.2em] mb-3 uppercase">La Nostra Storia</h2>
        <h3 class="text-4xl md:text-5xl font-black text-[var(--color-text-light)] uppercase tracking-tight mb-8">Our Story</h3>
        <p class="text-lg md:text-xl text-[var(--color-text-muted)] max-w-3xl mx-auto font-light leading-relaxed mb-10">
          Founded in Naples and brought to the heart of the city, Luxe Pizza is a celebration of authentic Italian culinary heritage. 
          We source the finest San Marzano tomatoes, premium Fior di Latte, and craft our dough daily using century-old techniques. 
          Experience the passion of true artisans.
        </p>
        <button class="bg-transparent border-2 border-[var(--color-accent-gold)] text-[var(--color-accent-gold)] px-8 py-3 rounded-full font-bold uppercase tracking-widest hover:bg-[var(--color-accent-gold)] hover:text-black transition-all duration-300 cursor-pointer">
          Discover More
        </button>
      </div>
    </section>
  </div>
</template>

<script setup>
import Hero from '@/components/Hero.vue'
import MenuSection from '@/components/MenuSection.vue'
</script>
