<template>
  <footer class="bg-black pt-16 pb-8 border-t border-[var(--color-accent-gold)]/20">
    <div class="max-w-[1280px] mx-auto px-6">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-12 text-center md:text-left">
        
        <!-- Brand -->
        <div class="col-span-1 md:col-span-2">
          <a href="#" class="text-3xl font-black tracking-widest uppercase flex items-center justify-center md:justify-start gap-2 mb-6">
            <span class="text-[var(--color-accent-gold)] font-serif italic text-4xl">L</span>
            <span class="text-[var(--color-text-light)]">UXE PIZZA</span>
          </a>
          <p class="text-[var(--color-text-muted)] text-sm leading-relaxed max-w-sm mx-auto md:mx-0 font-light">
            Elevating the ancient art of Neapolitan pizza-making with premium ingredients, masterful technique, and a passion for perfection.
          </p>
        </div>

        <!-- Links -->
        <div>
          <h4 class="text-[var(--color-text-light)] font-bold tracking-widest uppercase mb-6 text-sm">Explore</h4>
          <ul class="space-y-4">
            <li><a href="#" class="text-[var(--color-text-muted)] hover:text-[var(--color-accent-gold)] transition-colors text-sm">Our Menu</a></li>
            <li><a href="#" class="text-[var(--color-text-muted)] hover:text-[var(--color-accent-gold)] transition-colors text-sm">Reservations</a></li>
            <li><a href="#" class="text-[var(--color-text-muted)] hover:text-[var(--color-accent-gold)] transition-colors text-sm">Private Events</a></li>
            <li><a href="#" class="text-[var(--color-text-muted)] hover:text-[var(--color-accent-gold)] transition-colors text-sm">Story</a></li>
          </ul>
        </div>

        <!-- Contact -->
        <div>
          <h4 class="text-[var(--color-text-light)] font-bold tracking-widest uppercase mb-6 text-sm">Contact</h4>
          <ul class="space-y-4 text-sm text-[var(--color-text-muted)]">
            <li>123 Luxury Avenue</li>
            <li>New York, NY 10012</li>
            <li class="pt-2">
               <a href="tel:+12125550198" class="text-[var(--color-accent-gold)] hover:text-yellow-400 transition-colors font-serif italic text-lg">+1 (212) 555-0198</a>
            </li>
            <li><a href="mailto:ciao@luxepizza.com" class="hover:text-[var(--color-text-light)] transition-colors">ciao@luxepizza.com</a></li>
          </ul>
        </div>
      </div>

      <!-- Bottom -->
      <div class="border-t border-white/10 mt-12 pt-8 flex flex-col md:flex-row items-center justify-between text-xs text-[var(--color-text-muted)]">
        <p>&copy; {{ new Date().getFullYear() }} Luxe Pizza. All rights reserved.</p>
        <div class="flex gap-6 mt-4 md:mt-0">
          <a href="#" class="hover:text-[var(--color-accent-gold)] transition-colors">Privacy Policy</a>
          <a href="#" class="hover:text-[var(--color-accent-gold)] transition-colors">Terms of Service</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
</script>
