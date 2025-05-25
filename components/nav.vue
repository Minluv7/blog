<template>
  <header class="shadow-lg z-50 bg-white relative">
    <div class="container mx-auto px-4 py-4 flex items-center justify-between">
      <!-- Logo -->
      <h1 class="text-[#013A63] font-bold uppercase text-2xl z-50">
        <NuxtLink to="/">Epiphany</NuxtLink>
      </h1>

     <!-- Hamburger knop -->
<div
  @click="menuOpen = !menuOpen"
  class="burger-inner md:hidden cursor-pointer w-8 h-6 flex flex-col justify-between z-50"
>
  <div
    class="top-bun h-0.5 bg-[#013A63] transition-all duration-300"
    :class="menuOpen ? 'rotate-45 translate-y-[12px]' : ''"
  ></div>
  <div
    class="patty h-0.5 bg-[#013A63] transition-all duration-300"
    :class="menuOpen ? 'opacity-0' : ''"
  ></div>
  <div
    class="bottom-bun h-0.5 bg-[#013A63] transition-all duration-300"
    :class="menuOpen ? '-rotate-45 -translate-y-2' : ''"
  ></div>
</div>


      <!-- Navigatie links (desktop) -->
      <nav class="hidden md:flex">
        <ul class="flex items-center text-[#013A63] gap-12">
          <li><NuxtLink to="/" exact-active-class="underline font-bold">Home</NuxtLink></li>
          <li><NuxtLink to="/about" exact-active-class="underline font-bold">About</NuxtLink></li>
          <li><NuxtLink to="/blog" exact-active-class="underline font-bold">Blog</NuxtLink></li>
        </ul>
      </nav>
    </div>

    <!-- Fullscreen navigatie overlay -->
    <transition name="fade">
      <div
        v-if="menuOpen"
        class="fixed inset-0 bg-white z-40 flex flex-col justify-center items-center space-y-8 text-[#013A63] text-2xl uppercase"
      >
        <NuxtLink to="/" exact-active-class="underline font-bold" @click="menuOpen = false">Home</NuxtLink>
        <NuxtLink to="/about" exact-active-class="underline font-bold" @click="menuOpen = false">About</NuxtLink>
        <NuxtLink to="/blog" exact-active-class="underline font-bold" @click="menuOpen = false">Blog</NuxtLink>
      </div>
    </transition>
  </header>
</template>

<script setup>
import { ref } from 'vue'
const menuOpen = ref(false)
</script>

<style scoped>

</style>
