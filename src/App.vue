<script setup lang="ts">
import HeaderComponent from "./components/HeaderComponent.vue";
import HomePage from "./pages/HomePage.vue";
import KnowledgesPage from "./pages/KnowledgesPage.vue";
import WorksPage from "./pages/WorksPage.vue";
import FooterPage from "./pages/FooterPage.vue";
import InfoPage from "./pages/InfoPage.vue";
</script>

<template>
  <HeaderComponent />
  <div class="flex flex-col items-stretch justify-start h-container font-geist">
    <HomePage />
    <KnowledgesPage />
    <InfoPage />
    <!-- <ProjetosPage /> -->
    <WorksPage />
    <FooterPage />
  </div>
</template>
