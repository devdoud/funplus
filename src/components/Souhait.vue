<script setup>
  import AddBasketButton from "./AddBasketButton.vue";

  defineProps({
    //image: String,
    text: String,
    point: parseInt,
    overpoint: String,
    status: String,

  })


</script>

<template>
  <div class="flex justify-start items-center">
    <div class="flex justify-start items-center mr-[2rem]">
      <img src="../assets/Image.png" alt="image drone" class="w-[4.5rem] h-[4.5rem]">
      <p class="font-jakarta font-medium text-sm text-test max-w-[12.63rem]">{{text}}</p>
    </div>

    <div class="w-[12.5rem] mr-[4rem]">
      <span class="text-sm font-public font-normal mr-1 text-[#929FA5] line-through">{{overpoint}}</span>
      <span class="text-sm font-public font-medium text-test">{{point}}k points</span>
    </div>

    <p class="font-public font-semibold text-sm text-green">{{status}}</p>

    <div class="flex items-center gap-4 ml-[8rem]">
      <AddBasketButton
          text="AJOUTER AU PANIER"
          bgColor="bg-[#ADB7BC]"
      />
      <img src="../assets/XCircle.png" alt="supprimer" class="w-[1.5rem] h-[1.5rem]">
    </div>

  </div>
</template>

<style scoped>

</style>