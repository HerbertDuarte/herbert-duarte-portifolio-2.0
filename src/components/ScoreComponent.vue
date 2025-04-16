<script setup lang="ts">
import InfoComponent from "./InfoComponent.vue";
function goToRepos() {
  window.open("https://github.com/HerbertDuarte?tab=repositories", "_blank");
}
</script>

<template>
  <div
    class="flex gap-10 xs:gap-16 flex-wrap items-center justify-center py-2 text-zinc-800"
  >
    <InfoComponent value="3">
      <p>
        Anos de <br />
        experiência
      </p>
    </InfoComponent>
    <div class="h-24 w-px bg-zinc-800"></div>

    <InfoComponent class="cursor-pointer" @click="goToRepos" value="65">
      <p>
        Repositórios <br />
        públicos
      </p>
    </InfoComponent>
    <div class="h-24 w-px bg-zinc-800"></div>
    <InfoComponent value="20h">
      <p>
        Cursos <br />
        ministrados
      </p>
    </InfoComponent>
  </div>
</template>
