<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
</script>

<template>
  <ContainerComponent theme="light">
    <div class="flex">
      <div class="flex-1 flex flex-col justify-center">
        <p class="font-lime text-4xl xs:text-5xl sm:text-6xl lg:text-7xl">
          Desenvolvedor Web & Arquiteto de Software
        </p>
        <p class="text-zinc-600 my-4">
          Sou um Arquiteto de Software & Desenvolvedor Full Stack Web,
          atualmente residindo em Vitória da Conquista, Bahia, Brasil.
        </p>
        <div class="my-4">
          <a
            href="https://www.linkedin.com/in/herbert-duarte-8534b71a2"
            target="_blank"
            class="flex justify-items-start items-center w-fit gap-1 bg-blue-500 font-medium text-white rounded-full py-3 px-6"
          >
            <img
              src="/images/linkedin.png"
              class="size-6 inline"
              alt="linkedin"
            />
            <span class="pb-px">LinkedIn</span>
          </a>
        </div>
        <p class="text-right font-madi text-3xl pt-2">
          <span class="text-6xl">H</span>erbert
          <span class="text-6xl">D</span>uarte
        </p>
      </div>
      <div class="flex-1 hidden lg:flex justify-end max-w-[35%] py-16">
        <div
          class="bg-zinc-50 size-[300px] 2xl:size-[350px] flex flex-col justify-end rounded-full"
        >
          <img
            class="w-full -translate-y-0 rounded-b-full"
            src="/images/herbert.png"
            alt="Herbert Duarte"
          />
        </div>
      </div>
    </div>
  </ContainerComponent>
</template>

<style scoped></style>
