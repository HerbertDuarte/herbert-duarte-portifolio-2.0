<script setup lang="ts">
type Theme = "dark" | "light" | "gray";
defineProps<{
  theme: Theme;
  className?: string;
}>();

const mapTheme: Record<Theme, string> = {
  light: "bg-white text-black",
  dark: "bg-black text-white",
  gray: "bg-zinc-50 text-zinc-950",
};
</script>
<template>
  <div :class="`w-full gap-8 p-6 ${mapTheme[theme]} ${className}`">
    <div class="max-w-[1280px] mx-auto">
      <slot />
    </div>
  </div>
</template>
