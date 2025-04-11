<script setup lang="ts"></script>

<template>
  <header class="py-4 px-6 fixed z-50 w-full backdrop-blur-md bg-white/70">
    <div
      class="flex items-center justify-between font-medium max-w-[1280px] mx-auto"
    >
      <p class="font-bold text-xl">Herbert.</p>
      <ul class="hidden sm:flex gap-4 items-center">
        <li class="text-blue-600">Home</li>
        <li>Experiências</li>
        <li>Conhecimentos</li>
        <li>Redes sociais</li>
      </ul>
      <a
        target="_blank"
        aria-label="Chat on WhatsApp"
        :href="`https://wa.me/77999851621`"
        class="bg-black text-white rounded-full py-2.5 px-3.5"
      >
        Fale comigo
      </a>
    </div>
  </header>
  <div class="h-20"></div>
</template>
