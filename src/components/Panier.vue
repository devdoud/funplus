<script setup>
import { ref } from 'vue'

import Souhait from "./Souhait.vue";
import AddBasketButton from "./AddBasketButton.vue";

const count = ref(1)
</script>

<template>
  <div class="w-[69rem] h-[30rem] bg-secondary mx-auto mt-3">
    <div class="w-full px-6 py-5 bg-white shadow">
      <p class="font-Plus+Jakarta+Sans font-bold text-xl leading-1.5 text-test">Panier</p>
    </div>

    <ul class="px-6 py-5 flex">
      <li class="mr-[14rem] font-medium text-sm text-test font-public">PRODUITS</li>
      <li class="mr-[14rem] font-medium text-sm text-test font-public">POINTS</li>
      <li class="mr-[14rem] font-medium text-sm text-test font-public">QUANTITE</li>
      <li class="mr-[14rem] font-medium text-sm text-test font-public">ACTIONS</li>
    </ul>

    <div class="w-full px-2 bg-white shadow h-full pt-5 flex flex-col gap-y-5">
      <div class="flex w-full items-start">
        <div class="w-2/3 p-6 flex flex-col gap-6">
          <div class="flex justify-start items-center">
            <div class="flex justify-start items-center mr-[2rem]">
              <img src="../assets/Image.png" alt="image drone" class="w-[4.5rem] h-[4.5rem]">
              <p class="font-jakarta font-medium text-sm text-test max-w-[12.63rem]">Bose Sport Earbuds - Wireless Earphones - Bluetooth In Ear Headphones for Workouts and Running, Triple Black</p>
            </div>

            <div class="w-[12.5rem] mr-[4rem]">
              <span class="text-sm font-public font-normal mr-1 text-[#929FA5] line-through">200K</span>
              <span class="text-sm font-public font-medium text-test">199k points</span>
            </div>

            <div class="flex justify-around items-center border border-gray-200 shadow w-[10.75rem] h-12 rounded-md">
              <button type="button" @click="count--">
                <img src="../assets/Minus.png" alt="Icone minus">
              </button>
              <span class="text-[#475156] text-base font-normal font-public">{{count}}</span>
              <button type="button" @click="count++">
                <img src="../assets/Plus.png" alt="Icone minus">
              </button>
            </div>

          </div>
        </div>
        <div class="p-6 h-full border-l border-gray-200 w-1/3">
          <div class="py-4 px-6">
            <p class="text-base font-public font-medium">Total articles</p>
          </div>
          <div class="flex flex-col gap-1.5 border-b border-gray-200 pb-4">
            <div class=" flex justify-between">
              <span class="font-jakarta text-sm text-[#4C4C4C]">Sous Total</span>
              <span class="font-public font-medium text-sm text-[#191C1F]">3.198M</span>
            </div>

            <div class=" flex justify-between">
              <span class="font-jakarta text-sm text-[#4C4C4C]">Sous Total</span>
              <span class="font-public font-medium text-sm text-[#191C1F]">3.198M</span>
            </div>

            <div class=" flex justify-between">
              <span class="font-jakarta text-sm text-[#4C4C4C]">Sous Total</span>
              <span class="font-public font-medium text-sm text-[#191C1F]">Gratuit</span>
            </div>

            <div class=" flex justify-between">
              <span class="font-jakarta text-sm text-[#4C4C4C]">Sous Total</span>
              <span class="font-public font-medium text-sm text-[#191C1F]">3.198M</span>
            </div>
          </div>

          <div class=" flex justify-between my-4">
            <span class="font-jakarta font-medium text-sm text-[#4C4C4C]">Total</span>
            <span class="font-public font-medium text-sm text-[#191C1F]">3.198M Points</span>
          </div>

          <AddBasketButton
            text="RETIRER MA COMMANDE"
            width="w-[20rem]"
          />
        </div>
      </div>
    </div>
  </div>

</template>

<style scoped>

</style>