<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import WorkComponent from "../components/WorkComponent.vue";
import type { Work } from "../components/WorkComponent.vue";

const works: Work[] = [
  {
    title: "Tivic - Tecnologia da Informação",
    subtitle: "Junior 3 | 04/2024 - NOW",
    items: [
      "Software Architecture",
      "Web Fullstack Development",
      "Team Management",
      "SPRING | NESTJS | ANGULAR",
    ],
  },

  {
    title: "OOISME",
    subtitle: "Freelance | 01/2025 - 04/2025",
    items: ["Web Fullstack Development", "Web Security", "NEXTJS | NESTJS"],
  },

  {
    title: "City Hall of Vitória da Conquista",
    subtitle: "Intern | 08/2023 - NOW",
    items: ["Web Fullstack Development", "VUEJS | NESTJS"],
  },

  {
    title: "Açaí Flash",
    subtitle: "Freelance | 01/2024 - 04/2024",
    items: ["Tech Lead", "Web Fullstack Development", "VUEJS | NESTJS"],
  },
];
</script>
<template>
  <ContainerComponent theme="gray">
    <div class="flex flex-col gap-8 font-serif pb-6">
      <div
        class="text-2xl font-semibold py-4 flex justify-center items-center gap-3"
      >
        <span class="h-[2px] flex-1 max-w-20 bg-zinc-900" />
        <p>Work Experience</p>
        <span class="h-[2px] flex-1 max-w-20 bg-zinc-900" />
      </div>

      <div
        class="flex items-start flex-wrap flex-col md:flex-row justify-center gap-14"
      >
        <WorkComponent
          :work="work"
          :key="index"
          v-for="(work, index) in works"
        />
      </div>
    </div>
  </ContainerComponent>
</template>
