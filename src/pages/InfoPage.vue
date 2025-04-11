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
      class="flex font-serif gap-16 flex-wrap items-center justify-around py-2"
    >
      <InfoComponent value="3">
        Years of <br />
        experience
      </InfoComponent>
      <InfoComponent class="cursor-pointer" @click="goToRepos" value="65">
        Public <br />repositories
      </InfoComponent>
      <InfoComponent value="20h">
        Courses <br />
        taught
      </InfoComponent>
    </div>
  </ContainerComponent>
</template>
