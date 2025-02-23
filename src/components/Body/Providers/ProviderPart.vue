<template>
  <div
    class="flex justify-between mx-[20px] md:mx-[50px] 2xl:mx-[240px] max-w-[1440px] items-center text-white my-[20px]"
  >
    <span class="text-[32px] font-semibold">All Providers</span>
    <span class="flex items-center text-[15px] font-normal">
      SEE ALL
      <all-icon class="ml-[10px]" />
    </span>
  </div>
  <div
    class="flex mx-[20px] md:mx-[50px] 2xl:mx-[240px] overflow-y-auto max-w-[1440px] gap-5 justify-around"
  >
    <provider-item
      v-for="(provider, index) in listProvider"
      :title="provider.title"
      :amount="provider.amount"
      :key="index"
    />
  </div>
</template>
<script setup>
import ProviderItem from './ProviderItem.vue'
import AllIcon from './Icon/AllIcon.vue'
const listProvider = [
  {
    title: 'Evolution',
    amount: 312,
  },
  {
    title: 'Spribe',
    amount: 12,
  },
  {
    title: 'VeliPlay',
    amount: 9,
  },
  {
    title: 'Turbo Games',
    amount: 36,
  },
  {
    title: 'SmartSoft',
    amount: 37,
  },
  {
    title: '100HP Gaming',
    amount: 7,
  },
  {
    title: 'BGaming',
    amount: 166,
  },
  {
    title: 'Wazdan',
    amount: 199,
  },
]
</script>
