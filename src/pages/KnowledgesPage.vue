<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import "/src/assets/angular.png";
import "/src/assets/vue.webp";
import "/src/assets/nest.png";
import "/src/assets/springboot.png";
import "/src/assets/nuxt.png";
import "/src/assets/next.png";
import "/src/assets/postgres.png";
</script>
<template>
  <ContainerComponent theme="light">
    <div class="flex flex-col gap-8 font-serif">
      <div class="flex items-center justify-center gap-6 flex-wrap">
        <div class="h-9">
          <img class="h-full" src="/src/assets/nest.png" alt="nest" />
        </div>
        <div class="h-10">
          <img
            class="h-full"
            src="/src/assets/springboot.png"
            alt="springboot"
          />
        </div>

        <div class="h-9">
          <img class="h-full" src="/src/assets/angular.png" alt="angular" />
        </div>

        <div class="h-11">
          <img class="h-full" src="/src/assets/vue.webp" alt="vue" />
        </div>

        <div class="h-9">
          <img class="h-full" src="/src/assets/nuxt.png" alt="nuxt" />
        </div>

        <div class="h-4.5 my-4">
          <img class="h-full" src="/src/assets/next.png" alt="next" />
        </div>

        <div class="h-10">
          <img class="h-full" src="/src/assets/postgres.png" alt="postgres" />
        </div>
      </div>
    </div>
  </ContainerComponent>
</template>
