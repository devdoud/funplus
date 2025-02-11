<script setup>
  defineProps({
    description: String,
  })
</script>

<template>
  <div class="flex flex-col gap-0.5 items-center justify-center">
    <img src="../assets/Notebook.png" alt="notebook" class="w-8 h-8" />
    <p class="font-semibold text-sm text-[#191C1F] font-jakarta">{{description}}</p>
  </div>
</template>

<style scoped>

</style>