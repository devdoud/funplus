<script setup>

import Activite from "./Activite.vue";

</script>

<template>
    <div class="w-[69rem] bg-secondary mx-auto mt-3 p-6 flex flex-col gap-6">
       <div class="bg-primary flex items-center justify-between px-6 rounded-2xl w-full h-[11rem]">
            <div class="flex flex-col gap-1">
              <p class="font-jakarta font-semibold text-[#FFF6E2] text-2xl">#Commande Nº96459761</p>
              <div class="flex gap-1.5">
                <span class="font-public font-normal text-xs text-white">49 Products</span>
                <span class="font-public font-normal text-xs text-white">Achats effectués ce 02 Février 2025</span>
              </div>
            </div>
            <span class="text-[#FAA949] font-public font-extrabold text-4xl">3 198 000 points </span>
       </div>

      <p class="font-jakarta font-semibold text-base">Vos produit seront disponible au point de collecte le 14 Février 2025</p>

      <div class="pb-6 flex flex-col items-center gap-6 border-b border-gray-200">

      </div>

      <div class="flex flex-col items-start">
        <p class="font-jakarta font-bold text-sm text-[#191C1F] mb-6">Activité de la commande</p>
        <div class="flex flex-col items-start gap-4">
          <Activite />
          <Activite />
          <Activite />
        </div>
      </div>

    </div>
</template>

<style scoped>

</style>background: #191C1F;
