<template>
  <nav class="sticky top-0 z-50 bg-[var(--color-primary-dark)]/95 backdrop-blur-md border-b-2 border-[var(--color-accent-gold)]/20 shadow-[0_4px_30px_rgba(0,0,0,0.5)] transition-all duration-300">
    <div class="max-w-[1280px] mx-auto px-6 h-20 flex items-center justify-between">
      <!-- Logo -->
      <a href="#" class="text-2xl font-black tracking-widest uppercase flex items-center gap-2">
        <span class="text-[var(--color-accent-gold)] font-serif italic text-3xl">L</span>
        <span class="text-[var(--color-text-light)]">UXE PIZZA</span>
      </a>

      <!-- Desktop Links -->
      <div class="hidden md:flex items-center gap-8">
        <a v-for="link in links" :key="link.name" :href="link.href" class="text-sm font-medium tracking-wider text-[var(--color-text-muted)] hover:text-[var(--color-accent-gold)] transition-colors duration-300 relative group uppercase">
          {{ link.name }}
          <span class="absolute -bottom-1 left-0 w-0 h-0.5 bg-[var(--color-accent-gold)] transition-all duration-300 group-hover:w-full"></span>
        </a>
      </div>

      <!-- CTA Button -->
      <button class="hidden md:block bg-gradient-to-r from-[var(--color-accent-gold)] to-yellow-600 text-black px-6 py-2.5 rounded-full font-bold uppercase tracking-wide text-sm hover:scale-105 hover:shadow-[0_0_15px_rgba(212,175,55,0.4)] transition-all duration-300 cursor-pointer">
        Order Now
      </button>

      <!-- Mobile Menu Button -->
      <button class="md:hidden text-[var(--color-text-light)] hover:text-[var(--color-accent-gold)] p-2">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-8 h-8">
          <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
        </svg>
      </button>
    </div>
  </nav>
</template>

<script setup>
const links = [
  { name: 'Home', href: '#' },
  { name: 'Menu', href: '#menu' },
  { name: 'About', href: '#about' },
  { name: 'Contact', href: '#contact' },
]
</script>
