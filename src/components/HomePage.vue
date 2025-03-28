<script setup lang="ts">
import { ArrowRightIcon } from "lucide-vue-next";
</script>

<template>
  <div class="w-full max-w-[1000px] mx-auto flex gap-8 p-6">
    <div class="bg-black h-[450px] w-[300px] rounded-full"></div>
    <div class="flex-1 flex flex-col justify-around">
      <p class="font-lime text-7xl">Software Architect & Web Developer</p>
      <p class="text-zinc-600">
        I'm a Full Stack Software Architect & Creative Web Developer based in
        Vitória da Conquista, Bahia, Brazil.
      </p>
      <div class="my-4">
        <button
          class="bg-blue-500 font-medium text-white rounded-full py-3 px-6"
        >
          About me <ArrowRightIcon :size="18" class="inline" />
        </button>
      </div>
      <p class="font-madi text-3xl">
        <span class="text-6xl">H</span>erbert
        <span class="text-6xl">D</span>uarte
      </p>
    </div>
  </div>
</template>
