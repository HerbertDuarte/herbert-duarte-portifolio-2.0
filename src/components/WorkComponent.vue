<script setup lang="ts">
export type Work = {
  title: string;
  subtitle: string;
  items: string[];
};

defineProps<{
  work: Work;
}>();
</script>
<template>
  <div class="space-y-4">
    <div>
      <p class="font-semibold">{{ work.title }}</p>
      <p class="text-sm font-sans">{{ work.subtitle }}</p>
    </div>

    <ul class="list-disc list-inside italic">
      <li v-for="item in work.items">{{ item }}</li>
    </ul>
  </div>
</template>
