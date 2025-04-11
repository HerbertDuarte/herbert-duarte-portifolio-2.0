<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import InfoComponent from "../components/InfoComponent.vue";

function goToRepos() {
  window.open("https://github.com/HerbertDuarte?tab=repositories", "_blank");
}
</script>

<template>
  <ContainerComponent theme="dark">
    <div
      class="flex font-serif gap-16 flex-wrap items-center justify-around py-2 text-zinc-200"
    >
      <InfoComponent value="3">
        <p>
          Anos de <br />
          experiência
        </p>
      </InfoComponent>
      <InfoComponent class="cursor-pointer" @click="goToRepos" value="65">
        <p>
          Repositórios <br />
          públicos
        </p>
      </InfoComponent>
      <InfoComponent value="20h">
        <p>
          Cursos <br />
          ministrados
        </p>
      </InfoComponent>
    </div>
  </ContainerComponent>
</template>
