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
      :icon="provider.icon"
    />
  </div>
</template>
<script setup>
import ProviderItem from './ProviderItem.vue'
import AllIcon from './Icon/AllIcon.vue'
import EvolutionIcon from './Icon/EvolutionIcon.vue'
import SpribeIcon from './Icon/SpribeIcon.vue'
import VeliPlayIcon from './Icon/VeliPlayIcon.vue'
import TurboGamesIcon from './Icon/TurboGamesIcon.vue'
import SmartSoftIcon from './Icon/SmartSoftIcon.vue'
import HPGamingIcon from './Icon/HPGamingIcon.vue'
import BGamingIcon from './Icon/BGamingIcon.vue'
import WazdanIcon from './Icon/WazdanIcon.vue'

const listProvider = [
  {
    title: 'Evolution',
    amount: 312,
    icon: EvolutionIcon,
  },
  {
    title: 'Spribe',
    amount: 12,
    icon: SpribeIcon,
  },
  {
    title: 'VeliPlay',
    amount: 9,
    icon: VeliPlayIcon,
  },
  {
    title: 'Turbo Games',
    amount: 36,
    icon: TurboGamesIcon,
  },
  {
    title: 'SmartSoft',
    amount: 37,
    icon: SmartSoftIcon,
  },
  {
    title: '100HP Gaming',
    amount: 7,
    icon: HPGamingIcon,
  },
  {
    title: 'BGaming',
    amount: 166,
    icon: BGamingIcon,
  },
  {
    title: 'Wazdan',
    amount: 199,
    icon: WazdanIcon,
  },
]
</script>
