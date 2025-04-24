<script setup lang="ts">
import { LinkIcon } from "lucide-vue-next";
import ContainerComponent from "../components/ContainerComponent.vue";
import type { SocialButtonProps } from "../components/SocialCircleButtonComponent.vue";
import SocialCircleButtonComponent from "../components/SocialCircleButtonComponent.vue";

type Tool = {
  link: string;
  label: string;
};

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

const tools: Tool[] = [
  {
    label: "Calculadora de Média Final - IFBA",
    link: "https://mediafinal-ifba.vercel.app/",
  },
  {
    label: "Repart - Play Match Generator",
    link: "https://repart.vercel.app/",
  },
  {
    label: "Criptovue - Cotação e Conversão de Moedas",
    link: "https://cryptovue-ochre.vercel.app/",
  },
];
</script>
<template>
  <ContainerComponent theme="dark">
    <div
      class="flex flex-col sm:flex-row items-start justify-between gap-10 sm:gap-20 flex-wrap text-zinc-300"
    >
      <div class="flex justify-between flex-1 flex-wrap gap-6">
        <div>
          <p class="uppercase text-zinc-500 pb-3">Email</p>
          <p>herbertduarte.santos@gmail.com</p>
        </div>

        <div>
          <p class="uppercase text-zinc-500 pb-3">Serviços</p>
          <p>Planejamento de projeto</p>
          <p>Desenvolvimento de software</p>
          <p>Liderança técnica</p>
          <p>Capacitação</p>
        </div>

        <div>
          <p class="uppercase text-zinc-500 pb-3">LINKS</p>
          <p
            class="flex items-start gap-2 hover:underline hover:text-blue-200"
            v-for="(tool, index) in tools"
            :key="index"
          >
            <LinkIcon class="mt-[2px]" :size="18" />
            <a :href="tool.link">{{ tool.label }}</a>
          </p>
        </div>
      </div>
      <div class="space-y-2">
        <p class="uppercase text-zinc-500 pb-3">Redes sociais</p>
        <div class="flex justify-center items-center gap-2">
          <SocialCircleButtonComponent
            v-for="(button, index) in socialButtons"
            :item="button"
            :key="index"
          />
        </div>
      </div>
    </div>

    <div class="text-sm pt-12">&copy; 2025 Herbert Duarte</div>
  </ContainerComponent>
</template>
