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
          "Em uma das minhas experiências participei da construção dos sistemas
          de processamento de fluxo e infrações de trânsito para mais de 14
          cidades incluindo Belo Horizonte que é a 3° maior do Brasil em
          tráfego. Várias estratégias foram usadas para conseguir lidar com a
          grande carga dessas cidades, pude participar de decisões técnicas e
          liderar a equipe."
        </p>
        <p>
          "Em outra experiência, no início da minha carreira, pude planejar e
          construir um sistema de gestão de tarefas e projetos para prefeituras.
          Hoje (outubro de 2025) o sistema é fortemente usado por duas das 3
          maiores cidades da Bahia, sendo de suma importância para documentação
          e controle dos projetos e cumprimento de prazos, pois é baseado em
          gráficos gantt que foram construídos manualmente, sem uso de
          bibliotecas para atender precisamente às necessidades das
          prefeituras."
        </p>

        <p>
          "Também tenho alguns materiais didáticos postados no Youtube e tive a
          honra de ministrar um minicurso sobre TDD (Test-Driven Development) e
          DDD (Domain-Driven Design) no IFBA - Instituto Federal da Bahia,
          Campus de Vitória da Conquista na Week IT 2024."
        </p>
      </div>
    </div>
  </ContainerComponent>
</template>
