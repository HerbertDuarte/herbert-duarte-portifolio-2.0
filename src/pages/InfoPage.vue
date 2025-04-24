<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import CardProjectComponent, {
  type Projeto,
} from "../components/CardProjectComponent.vue";
import { ref, computed } from "vue";

const projetos: Projeto[] = [
  {
    name: "Live - Fundamentos Vue 3",
    description:
      "Uma live no Youtube onde ensino os fundamentos do framework Vue JS.",
    src: "/images/live-vue.jpg",
    link: "https://www.youtube.com/watch?v=Enqjp5hXsV8",
  },
  {
    name: "GanttHub",
    description:
      "Sistema de gestão de projetos para a Prefeitura de Vitoria da Conquista.",
    src: "/images/gantthub2.png",
  },
  {
    name: "Açaí Flash - Sorteios",
    description: "Sistema de sorteios para uma rede de lojas de açaí.",
    src: "/images/acai-flash.png",
  },
  {
    name: "Ana Clara - Modelo de publicidade",
    description:
      "Uma landing page para um modelo de publicidade. Projeto de estudo do React JS.",
    src: "/images/ana-clara2.png",
    link: "https://anaclara-model.vercel.app/",
  },
];
const sm = 640;
const isMobile = ref(window.innerWidth < sm);

window.addEventListener("resize", () => {
  isMobile.value = window.innerWidth < sm;
});

const displayedProjects = computed(() => {
  return isMobile.value ? projetos.slice(0, 3) : projetos;
});
</script>

<template>
  <ContainerComponent theme="gray">
    <div
      class="text-2xl font-semibold py-4 flex justify-center items-center gap-3 font-serif italic"
    >
      <span class="h-[2px] flex-1 max-w-20 bg-zinc-900" />
      <p>Alguns projetos</p>
      <span class="h-[2px] flex-1 max-w-20 bg-zinc-900" />
    </div>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 py-4">
      <CardProjectComponent
        :projeto="projeto"
        :key="index"
        v-for="(projeto, index) in displayedProjects"
      />
    </div>
  </ContainerComponent>
</template>
