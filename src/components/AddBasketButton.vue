<script setup>
  import { computed } from 'vue';

  const props = defineProps({
    text: String,
    bgColor: {
      type: String,
      default: 'bg-[#32756C]'
    },
    width: {
      type: String,
      default: 'w-[13.8rem]'
    }
  });

  const buttonClass = computed(() => `${props.bgColor} ${props.width}`);

</script>

<template>
  <button 
    :class="buttonClass"
    class="h-12 rounded-xl text-white flex items-center justify-center gap-1 font-public font-bold text-sm"
  >
    {{ text }}
    <img src="../assets/ShoppingCartSimple.png" alt="Shopping Cart" class="w-[1.25rem] h-[1.25rem]">
  </button>
</template>

<style scoped>

</style>