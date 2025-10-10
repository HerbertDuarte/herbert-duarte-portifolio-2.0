<script setup lang="ts">
defineProps<{
  title: string;
}>();
</script>

<template>
  <div
    class="text-2xl font-semibold py-4 flex justify-center items-center gap-3 font-serif"
  >
    <span class="h-[2px] flex-1 max-w-20 bg-zinc-900" />
    <p>{{ title }}</p>
    <span class="h-[2px] flex-1 max-w-20 bg-zinc-900" />
  </div>
</template>
