<script setup lang="ts">
defineProps<{
  value: string;
}>();
</script>

<template>
  <div class="text-center space-y-2">
    <p class="text-3xl xs:text-4xl sm:text-5xl">
      <span class="text-3xl">+</span>{{ value }}
    </p>
    <p class="italic">
      <slot />
    </p>
  </div>
</template>
