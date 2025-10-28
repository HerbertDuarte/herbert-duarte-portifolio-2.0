<script setup lang="ts">
import ContainerComponent from "../components/ContainerComponent.vue";
import TitleComponent from "../components/TitleComponent.vue";
</script>
<template>
  <ContainerComponent theme="light">
    <TitleComponent title="Highlights" />

    <div class="flex justify-center py-4 sm:py-6 px-0 xs:px-2 sm:px-6 md:px-8">
      <div class="italic space-y-8 indent-8 max-w-4xl font-serif text-zinc-700">
        <p>
          "Em umas das minhas experiências, pude arquitetar e desenvolver do
          zero um serviço de autenticação e permissões usando conceitos de RBAC
          e ABAC, NestJS, Postgres, JWT, OAuth2 e TFA com confirmação via email.
          Tudo isso utilizando boas práticas de segurança como cookies httpOnly,
          recaptcha e prevenção de brute force. Todo o sistema foi desenvolvido
          utilizando boas práticas de SOLID, Design Patterns, TDD com Testes de
          integração e Clean Architecture."
        </p>
        <p>
          "Para integrar a parte das permissões em outros sistemas Java e
          SpringBoot criei uma biblioteca que continha anotações para serem
          usadas em controllers como Guards das rotas. Também adicionei
          utilitários que facilitam a comunicação com o serviço, para consulta
          de informações dos usuários, seus grupos e suas permissões."
        </p>

        <p>
          "Para integrar a parte das permissões em outros sistemas Java e
          SpringBoot criei uma biblioteca que continha anotações para serem
          usadas em controllers como Guards das rotas. Também adicionei
          utilitários que facilitam a comunicação com o serviço, para consulta
          de informações dos usuários, seus grupos e suas permissões."
        </p>
        <p>
          "Automatizei também processos de deploy, e o fluxo de desenvolvimento
          da equipe com ferramentas como Coolify, WebHooks e Github actions.
          Economizando o tempo de desenvolvimento e testes, reduzindo a
          necessidade de abertura de cards unicamente para deploys em ambientes
          de teste e homologação e possibilitando com que toda a equipe possa
          participar desse processo com uma baixa curva de aprendizagem."
        </p>
      </div>
    </div>
  </ContainerComponent>
</template>
