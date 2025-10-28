<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";

const technologies = [
  { src: "/images/nest.png", alt: "nest", height: "h-9" },
  { src: "/images/springboot.png", alt: "springboot", height: "h-10" },
  { src: "/images/angular.png", alt: "angular", height: "h-9" },
  { src: "/images/vue.webp", alt: "vue", height: "h-11" },
  { src: "/images/postgres.png", alt: "postgres", height: "h-10" },
  { src: "/images/redisdb.png", alt: "redisdb", height: "h-9" },
  { src: "/images/mongodb.png", alt: "mongodb", height: "h-11" },
  { src: "/images/docker.png", alt: "docker", height: "h-8" },
  { src: "/images/rabbitmq.png", alt: "rabbitmq", height: "h-5" },
];
</script>
<template>
  <ContainerComponent full-width theme="gray">
    <div class="carousel-container">
      <div class="carousel-track">
        <!-- Primeiro conjunto de imagens -->
        <div class="carousel-content">
          <div
            v-for="(tech, index) in technologies"
            :key="`tech-1-${index}`"
            :class="tech.height"
          >
            <img :src="tech.src" :alt="tech.alt" />
          </div>
        </div>
        <!-- Segundo conjunto de imagens (duplicado para efeito infinito) -->
        <div class="carousel-content">
          <div
            v-for="(tech, index) in technologies"
            :key="`tech-2-${index}`"
            :class="tech.height"
          >
            <img :src="tech.src" :alt="tech.alt" />
          </div>
        </div>
        <!-- Terceiro conjunto de imagens (garantir transição suave) -->
        <div class="carousel-content">
          <div
            v-for="(tech, index) in technologies"
            :key="`tech-3-${index}`"
            :class="tech.height"
          >
            <img :src="tech.src" :alt="tech.alt" />
          </div>
        </div>
      </div>
    </div>
  </ContainerComponent>
</template>

<style scoped>
.carousel-container {
  overflow: hidden;
  width: 100%;
  position: relative;
}

.carousel-track {
  display: flex;
  width: fit-content;
  animation: scroll 30s linear infinite;
}

.carousel-content {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  filter: grayscale(100%);
  padding: 0 0.75rem;
  flex-shrink: 0;
}

.carousel-content > div {
  flex-shrink: 0;
  display: inline-block;
}

.carousel-content img {
  display: block;
  height: 100%;
  width: auto;
  max-width: none;
  object-fit: contain;
}

@keyframes scroll {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(calc(-100% / 3));
  }
}

.carousel-track:hover {
  animation-play-state: paused;
}
</style>
