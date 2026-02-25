<template>
  <section class="relative w-full min-h-[80vh] flex items-center justify-center overflow-hidden">
    <!-- Background Texture -->
    <div class="absolute inset-0 z-0">
      <div class="absolute inset-0 bg-gradient-to-b from-[var(--color-primary-dark)]/80 via-transparent to-[var(--color-primary-dark)] z-10"></div>
      <img src="https://images.unsplash.com/photo-1513104890138-7c749659a591?q=80&w=2070&auto=format&fit=crop" alt="Delicious Pizza" class="w-full h-full object-cover object-center opacity-40 blur-[2px]" />
    </div>

    <!-- Content -->
    <div class="relative z-10 text-center px-4 max-w-4xl mx-auto flex flex-col items-center">
      <span class="text-[var(--color-accent-gold)] font-serif italic text-xl md:text-2xl mb-4 tracking-widest drop-shadow-md">Est. 1998</span>
      <h1 class="text-5xl md:text-7xl font-black text-[var(--color-text-light)] mb-6 uppercase tracking-tight leading-tight drop-shadow-2xl">
        Authentic <span class="text-transparent bg-clip-text bg-gradient-to-r from-[var(--color-accent-gold)] to-yellow-500">Italian</span><br/>Pizza Experience
      </h1>
      <p class="text-lg md:text-xl text-[var(--color-text-muted)] mb-10 max-w-2xl font-light">
        Wood-fired perfection crafted with zero-compromise ingredients. Taste the true essence of Napoli in every bite.
      </p>
      
      <div class="flex flex-col sm:flex-row gap-4 w-full sm:w-auto">
        <button class="bg-gradient-to-r from-[var(--color-accent-gold)] to-yellow-600 text-black px-8 py-4 rounded-full font-bold uppercase tracking-widest hover:scale-105 hover:shadow-[0_0_20px_rgba(212,175,55,0.6)] transition-all duration-300 cursor-pointer">
          View Menu
        </button>
        <button class="bg-transparent border-2 border-[var(--color-accent-gold)] text-[var(--color-accent-gold)] px-8 py-4 rounded-full font-bold uppercase tracking-widest hover:bg-[var(--color-accent-gold)] hover:text-black transition-all duration-300 cursor-pointer">
          Book Table
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>
