<script setup>
  import { computed } from 'vue';

  const props = defineProps({
    text: String,
    bgColor: {
      type: String,
      default: 'bg-[#32756C]'
    }
  });

  const buttonClass = computed(() => `${props.bgColor}`);

</script>

<template>
  <button 
    :class="buttonClass"
    class="max-w-96 h-[3rem] rounded-xl px-6 py-2 text-white flex items-center gap-1 font-public font-bold text-sm"
  >
    {{ text }}
    <img src="../assets/ShoppingCartSimple.png" alt="Shopping Cart" class="w-[1.25rem] h-[1.25rem]">
  </button>
</template>

<style scoped>

</style>