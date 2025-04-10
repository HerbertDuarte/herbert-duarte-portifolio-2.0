<script setup lang="ts">
export type SocialButtonProps = {
  linkUrl: string;
  imgUrl: string;
};
defineProps<{ item: SocialButtonProps }>();
</script>
<template>
  <a
    target="_blank"
    :href="item.linkUrl"
    class="size-10 rounded-full border p-1.5 opacity-65 hover:opacity-100 transition"
  >
    <img :src="item.imgUrl" />
  </a>
</template>
