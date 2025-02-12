<script setup>

import Souhait from "./Souhait.vue";
import AddBasketButton from "./AddBasketButton.vue";
</script>

<template>
  <div class="w-[69rem] h-[30rem] bg-secondary mx-auto mt-3">
    <div class="w-full px-6 py-5 bg-white shadow">
      <p class="font-Plus+Jakarta+Sans font-bold text-xl leading-1.5 text-test">Liste de souhaits</p>
    </div>

    <ul class="px-6 py-5 flex">
      <li class="mr-[14rem] font-medium text-sm text-test font-public">PRODUITS</li>
      <li class="mr-[14rem] font-medium text-sm text-test font-public">POINTS</li>
      <li class="mr-[14rem] font-medium text-sm text-test font-public">STATUS</li>
      <li class="mr-[14rem] font-medium text-sm text-test font-public">ACTIONS</li>
    </ul>

    <div class="w-full px-2 bg-white shadow h-full pt-5 flex flex-col gap-y-5">
      <Souhait
          image="../assets/Image.png"
          text="Bose Sport Earbuds - Wireless Earphones - Bluetooth In Ear Headphones for Workouts and Running, Triple Black"
          point={199}
          overpoint={299K}
          status="COLLECTÉS"
      >
        <template #add-basket-button>
          <AddBasketButton
              text="AJOUTER AU PANIER"
              bgColor="bg-[#32756C]"
          />
        </template>
      </Souhait>

      <Souhait
          image="../assets/Image.png"
          text="Bose Sport Earbuds - Wireless Earphones - Bluetooth In Ear Headphones for Workouts and Running, Triple Black"
          point={199}
          overpoint={299K}
          status="POINTS INSUFFISANTS"
      >
        <template #add-basket-button>
          <AddBasketButton
              text="AJOUTER AU PANIER"
              bgColor="bg-[#ADB7BC]"
          />
        </template>
      </Souhait>

      <Souhait
          image="../assets/Image.png"
          text="Bose Sport Earbuds - Wireless Earphones - Bluetooth In Ear Headphones for Workouts and Running, Triple Black"
          point={199}
          overpoint={299K}
          status="POINTS INSUFFISANTS"
      >
        <template #add-basket-button>
          <AddBasketButton
              text="AJOUTER AU PANIER"
              bgColor="bg-[#32756C]"
          />
        </template>
      </Souhait>

    </div>

  </div>
</template>

<style scoped>

</style>