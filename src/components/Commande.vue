<script setup>

import ProgressElement from "./ProgressElement.vue";
import Activite from "./Activite.vue";
</script>

<template>
  <div class="w-[69rem] p-6 bg-secondary mx-auto mt-3">

    <div class="bg-primary h-[10.75rem] rounded-3xl p-6 flex items-center justify-between mb-6">
        <div class="flex flex-col">
          <p class="text-[1.75rem] font-jakarta font-semibold text-[#FFF6E2]">#Commande Nº96459761</p>
          <div class="flex gap-2">
            <span class="text-sm font-normal font-public text-white">49 Products</span>
            <span class="text-sm font-normal font-public text-white">Achats effectués ce 02 Février 2025</span>
          </div>
        </div>
        <p class="text-orange font-jakarta font-extrabold text-4xl">3 198 000 points </p>
    </div>

    <p class="font-jakarta font-semibold text-base mb-6">Vos produit seront disponible au point de collecte le 14 Février 2025</p>

    <div class="flex flex-col items-center justify-center gap-2.5 pb-6 border-b border-gray-200">
      <img src="../assets/Progress.png" alt="progress image">
      <div class="flex gap-24">
        <ProgressElement
          description="Commande effectée"
        />
        <ProgressElement
            description="Commande effectée"
        />
        <ProgressElement
            description="Commande effectée"
        />
        <ProgressElement
            description="Commande effectée"
        />
      </div>
    </div>

    <div class="p-6 flex flex-col items-start">
      <p class="font-bold font-jakarta text-base mb-4">Activité de la commande</p>
      <div class="flex flex-col gap-3">
        <Activite />
        <Activite />
        <Activite />
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>