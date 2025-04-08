<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
</script>

<template>
  <ContainerComponent theme="light">
    <div class="flex">
      <div class="hidden flex-1 max-w-[35%]">
        <div class="bg-black h-[450px] w-[300px] rounded-full"></div>
      </div>
      <div class="flex-1 flex flex-col justify-center">
        <p class="font-lime text-5xl sm:text-6xl lg:text-7xl">
          Software Architect & Web Developer
        </p>
        <p class="text-zinc-600 my-4">
          I'm a Full Stack Software Architect & Creative Web Developer based in
          Vitória da Conquista, Bahia, Brazil.
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
    </div>
  </ContainerComponent>
</template>
