<script setup lang="ts">
import { Link2Icon } from "lucide-vue-next";
import ContainerComponent from "../components/ContainerComponent.vue";
import WorkComponent from "../components/WorkComponent.vue";
import type { Work } from "../components/WorkComponent.vue";
import TitleComponent from "../components/TitleComponent.vue";

const works: Work[] = [
  {
    title: "Tivic - Tecnologia da Informação",
    subtitle: "Pleno / Coordenador (Abr 2024 - Presente)",
    items: [
      "Arquitetura de Software",
      "Desenvolvimento Web Fullstack",
      "Gestão de Equipe",
      "SPRINGBOOT | NESTJS | ANGULAR",
    ],
  },

  {
    title: "OOISME",
    subtitle: "Freelancer (Jan 2025 - Abr 2025)",
    items: [
      "Desenvolvimento Web Fullstack",
      "Segurança Web",
      "NEXTJS | NESTJS",
    ],
  },

  {
    title: "Prefeitura de Vitória da Conquista",
    subtitle: "Estagiário (Ago 2023 - Presente)",
    items: [
      "Desenvolvimento Web Fullstack",
      "VUEJS | NESTJS",
      "QUASAR FRAMEWORK",
    ],
  },

  // {
  //   title: "Açaí Flash",
  //   subtitle: "Freelancer (Jan 2024 - Abr 2024)",
  //   items: ["Líder Técnico", "Desenvolvimento Web Fullstack", "VUEJS | NESTJS"],
  // },
];
</script>
<template>
  <ContainerComponent theme="light">
    <div class="flex flex-col gap-8 font-serif pb-6">
      <TitleComponent title="Experiência Profissional" />

      <div
        class="flex items-start flex-wrap flex-col md:flex-row justify-center lg:justify-between gap-14"
      >
        <WorkComponent
          :work="work"
          :key="index"
          v-for="(work, index) in works"
        />
      </div>

      <div>
        <a
          class="hover:underline flex items-center gap-2"
          target="_blank"
          href="https://docs.google.com/document/d/1xD3qLXELNHdc2V1awa9_ZEwPjAd_cNeviG6fy68tXwU"
        >
          <Link2Icon :size="18" />
          <span>Ver currículo</span>
        </a>
      </div>
    </div>
  </ContainerComponent>
</template>
