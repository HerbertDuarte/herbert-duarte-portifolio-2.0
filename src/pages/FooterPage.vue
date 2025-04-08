<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import type { SocialButtonProps } from "../components/SocialCircleButtonComponent.vue";
import SocialCircleButtonComponent from "../components/SocialCircleButtonComponent.vue";

const socialButtons: SocialButtonProps[] = [
  {
    imgUrl: "/images/linkedin.png",
    linkUrl: "https://www.linkedin.com/in/herbert-duarte-8534b71a2",
  },

  {
    imgUrl: "/images/github.png",
    linkUrl: "https://github.com/HerbertDuarte",
  },

  {
    imgUrl: "/images/youtube.png",
    linkUrl: "https://www.youtube.com/@herbertduarte_dev",
  },
];
</script>
<template>
  <ContainerComponent theme="dark">
    <div class="space-y-4">
      <div class="flex justify-center items-center gap-2">
        <SocialCircleButtonComponent
          v-for="(button, index) in socialButtons"
          :item="button"
          :key="index"
        />
      </div>
      <p class="text-center">herbertduarte.santos@gmail.com</p>
    </div>
  </ContainerComponent>
</template>
