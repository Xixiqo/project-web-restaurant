<template>
  <section id="menu" class="py-24 bg-[var(--color-primary-dark)]">
    <div class="max-w-[1280px] mx-auto px-6">
      
      <!-- Section Header -->
      <div class="text-center mb-16">
        <h2 class="text-sm font-serif italic text-[var(--color-accent-gold)] tracking-[0.2em] mb-3 uppercase">Signatures</h2>
        <h3 class="text-4xl md:text-5xl font-black text-[var(--color-text-light)] uppercase tracking-tight">Our Premium Selection</h3>
        <div class="w-24 h-1 bg-[var(--color-accent-gold)] mx-auto mt-6 rounded-full opacity-60"></div>
      </div>

      <!-- Menu Grid -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10">
        <div v-for="pizza in menuItems" :key="pizza.id" class="group bg-[var(--color-primary-light)] rounded-2xl overflow-hidden border border-[var(--color-accent-gold)]/10 hover:border-[var(--color-accent-gold)]/50 transition-all duration-500 hover:-translate-y-2 hover:shadow-[0_15px_30px_rgba(0,0,0,0.6)]">
          <!-- Image -->
          <div class="relative h-64 overflow-hidden">
            <div class="absolute inset-0 bg-black/20 group-hover:bg-transparent transition-all duration-500 z-10"></div>
            <img :src="pizza.image" :alt="pizza.name" class="w-full h-full object-cover transform group-hover:scale-110 transition-transform duration-700 ease-out" />
            <div class="absolute top-4 right-4 z-20 bg-[var(--color-primary-dark)]/90 backdrop-blur-sm text-[var(--color-accent-gold)] px-4 py-1.5 rounded-full font-bold border border-[var(--color-accent-gold)]/30">
              {{ pizza.price }}
            </div>
          </div>
          
          <!-- Details -->
          <div class="p-8">
            <h4 class="text-2xl font-bold text-[var(--color-text-light)] mb-3 uppercase group-hover:text-[var(--color-accent-gold)] transition-colors">{{ pizza.name }}</h4>
            <p class="text-[var(--color-text-muted)] mb-6 text-sm leading-relaxed font-light">{{ pizza.description }}</p>
            <div class="flex items-center justify-between mt-auto">
              <span class="text-xs uppercase tracking-widest text-[var(--color-accent-gold)]/80 font-semibold">{{ pizza.calories }} kcal</span>
              <button class="text-[var(--color-text-light)] hover:text-white bg-[var(--color-accent-maroon)] hover:bg-red-800 px-5 py-2 rounded-full text-sm font-semibold uppercase tracking-wider transition-all duration-300">
                Add to Cart
              </button>
            </div>
          </div>
        </div>
      </div>
      
      <div class="text-center mt-16">
        <button class="text-[var(--color-text-light)] hover:text-[var(--color-accent-gold)] border-b border-[var(--color-accent-gold)] pb-1 font-medium tracking-widest uppercase transition-all">
          Explore Full Menu &rarr;
        </button>
      </div>

    </div>
  </section>
</template>

<script setup>
const menuItems = [
  {
    id: 1,
    name: "Truffle Mushroom",
    description: "Wild mushrooms, white truffle oil, fior di latte, aged parmesan, and a touch of fresh thyme.",
    price: "$28",
    calories: "780",
    image: "https://images.unsplash.com/photo-1513104890138-7c749659a591?q=80&w=800&auto=format&fit=crop"
  },
  {
    id: 2,
    name: "Classic Margherita",
    description: "San Marzano tomato sauce, fresh buffalo mozzarella, fragrant basil leaves, and extra virgin olive oil.",
    price: "$22",
    calories: "650",
    image: "https://images.unsplash.com/photo-1574071318508-1cdbab80d002?q=80&w=800&auto=format&fit=crop"
  },
  {
    id: 3,
    name: "Spicy Diavola",
    description: "Spicy calabrese salami, crushed red pepper flakes, fresh mozzarella, and hot honey drizzle.",
    price: "$26",
    calories: "820",
    image: "https://images.unsplash.com/photo-1628840042765-356cda07504e?q=80&w=800&auto=format&fit=crop"
  }
]
</script>
