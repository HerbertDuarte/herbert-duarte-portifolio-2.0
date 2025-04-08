<script setup lang="ts">
import HeaderComponent from "./components/HeaderComponent.vue";
import HomePage from "./pages/HomePage.vue";
import KnowledgesPage from "./pages/KnowledgesPage.vue";
import WorksPage from "./pages/WorksPage.vue";
import FooterPage from "./pages/FooterPage.vue";
</script>

<template>
  <HeaderComponent />
  <div class="flex flex-col items-stretch justify-start h-container">
    <HomePage />
    <WorksPage />
    <KnowledgesPage />
    <div class="flex-1 bg-zinc-50"></div>
    <FooterPage />
  </div>
</template>
