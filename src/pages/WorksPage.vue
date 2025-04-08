<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import WorkComponent from "../components/WorkComponent.vue";
import type { Work } from "../components/WorkComponent.vue";

const works: Work[] = [
  {
    title: "Tivic - Tecnologia da Informação",
    subtitle: "Junior 3 (Apr 2024 - Present)",
    items: [
      "Software Architecture",
      "Web Fullstack Development",
      "Team Management",
      "SPRINGBOOT | NESTJS | ANGULAR",
    ],
  },

  {
    title: "OOISME",
    subtitle: "Freelance (Jan 2025 - Apr 2025)",
    items: ["Web Fullstack Development", "Web Security", "NEXTJS | NESTJS"],
  },

  {
    title: "City Hall of Vitória da Conquista",
    subtitle: "Intern (Aug 2023 - Present)",
    items: ["Web Fullstack Development", "VUEJS | NESTJS"],
  },

  {
    title: "Açaí Flash",
    subtitle: "Freelance (Jan 2024 - Apr 2024)",
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
        class="flex items-start flex-wrap flex-col md:flex-row justify-center lg:justify-between gap-14"
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
