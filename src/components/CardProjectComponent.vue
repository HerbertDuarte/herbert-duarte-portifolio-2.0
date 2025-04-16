<script setup lang="ts">
import { ArrowUpRight } from "lucide-vue-next";
export type Projeto = {
  name: string;
  description: string;
  src: string;
  link?: string;
};
defineProps<{ projeto: Projeto }>();

function redirectTo(link?: string) {
  if (link) {
    window.open(link, "_blank");
  }
}
</script>

<template>
  <div
    class="p-4 rounded-xl bg-white shadow-lg text-zinc-600 hover:scale-105 transition-all duration-300"
  >
    <img
      class="w-full aspect-[4/3] object-cover rounded-lg border border-zinc-50"
      :src="projeto.src"
      :alt="projeto.name"
    />
    <div class="pt-2 flex justify-between items-end gap-2">
      <div>
        <p class="font-bold">{{ projeto.name }}</p>
        <p>{{ projeto.description }}</p>
      </div>
      <button
        @click="redirectTo(projeto.link)"
        :disabled="!projeto.link"
        class="bg-blue-500 cursor-pointer text-white rounded-lg p-2 disabled:opacity-50 disabled:cursor-not-allowed"
      >
        <ArrowUpRight />
      </button>
    </div>
  </div>
</template>
