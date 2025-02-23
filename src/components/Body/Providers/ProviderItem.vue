<template>
  <div class="rounded-[10px]">
    <div class="bg-[#12294A] px-[30px] py-[15px]">
      <evolution-icon />
    </div>
    <div class="bg-[#1A3157] text-white text-center underline underline-offset-2 py-[10px]">
      <div>{{ props.title }}</div>
      <div>{{ props.amount }} games</div>
    </div>
  </div>
</template>
<script setup>
import EvolutionIcon from './Icon/EvolutionIcon.vue'
const props = defineProps({
  amount: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
})
</script>
