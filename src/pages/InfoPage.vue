<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";

function goToRepos() {
  window.open("https://github.com/HerbertDuarte?tab=repositories", "_blank");
}
</script>

<template>
  <ContainerComponent theme="dark">
    <div
      class="flex font-serif gap-16 flex-wrap items-center justify-around py-2"
    >
      <div class="text-center space-y-2">
        <p class="text-4xl sm:text-5xl"><span class="text-3xl">+</span>3</p>
        <p class="italic">
          Anos de <br />
          experiência
        </p>
      </div>

      <div @click="goToRepos" class="text-center space-y-2 cursor-pointer">
        <p class="text-4xl sm:text-5xl"><span class="text-3xl">+</span>65</p>
        <p class="italic">Repositórios <br />públicos</p>
      </div>

      <div class="text-center space-y-2">
        <p class="text-4xl sm:text-5xl"><span class="text-3xl">+</span>20h</p>
        <p class="italic">
          Cursos <br />
          ministrados
        </p>
      </div>
    </div>
  </ContainerComponent>
</template>
