<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import "/images/angular.png";
import "/images/vue.webp";
import "/images/nest.png";
import "/images/springboot.png";
import "/images/nuxt.png";
import "/images/next.png";
import "/images/postgres.png";
</script>
<template>
  <ContainerComponent theme="gray">
    <div class="flex flex-col gap-8 font-serif">
      <div
        class="flex items-center justify-center gap-6 flex-wrap filter grayscale"
      >
        <div class="h-9">
          <img class="h-full" src="/images/nest.png" alt="nest" />
        </div>
        <div class="h-10">
          <img class="h-full" src="/images/springboot.png" alt="springboot" />
        </div>

        <div class="h-9">
          <img class="h-full" src="/images/angular.png" alt="angular" />
        </div>

        <div class="h-11">
          <img class="h-full" src="/images/vue.webp" alt="vue" />
        </div>

        <div class="h-9">
          <img class="h-full" src="/images/nuxt.png" alt="nuxt" />
        </div>

        <div class="h-4.5 my-4">
          <img class="h-full" src="/images/next.png" alt="next" />
        </div>

        <div class="h-10">
          <img class="h-full" src="/images/postgres.png" alt="postgres" />
        </div>
      </div>
    </div>
  </ContainerComponent>
</template>
