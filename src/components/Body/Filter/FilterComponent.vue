<script setup>
import DiamondIcon from './Icons/DiamondIcon.vue'
import VipIcon from './Icons/VipIcon.vue'
import PromotionIcon from './Icons/PromotionIcon.vue'
import HotMatchIcon from './Icons/HotMatchIcon.vue'
import P2PIcon from './Icons/P2PIcon.vue'
import GameIcon from './Icons/GameIcon.vue'
import ProviderIcon from './Icons/ProviderIcon.vue'
</script>
<template>
  <div
    class="flex mx-[20px] md:mx-[50px] 2xl:mx-[240px] gap-1 md:gap-5 justify-between md:overflow-y-auto mt-[80px] text-white"
  >
    <span
      class="py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-[#90A2BD] justify-center hidden md:flex"
    >
      <diamond-icon class="mr-3" />
      <span>Diamond mine</span>
    </span>
    <span
      class="py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-[#90A2BD] justify-center hidden md:flex"
    >
      <vip-icon class="mr-3" />
      <span>VIP</span>
    </span>
    <span
      class="py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-[#90A2BD] justify-center hidden md:flex"
    >
      <promotion-icon class="mr-3" />
      <span>Promotion</span>
    </span>
    <span
      class="py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-[#90A2BD] justify-center hidden md:flex"
    >
      <hot-match-icon class="mr-3" />
      <span>Hot Match</span>
    </span>
    <span
      class="py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-[#90A2BD] justify-center hidden md:flex"
    >
      <P2P-icon class="mr-3" />
      <span>P2P Transaction</span>
    </span>
    <span
      class="py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-transparent justify-center bg-[#12294A] flex md:hidden items-center"
    >
      <span class="material-symbols-outlined mr-3"> search </span>

      <span>Search</span>
    </span>
    <span
      class="flex py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-transparent justify-center bg-[#12294A]"
    >
      <game-icon class="mr-3" />
      <span>Games</span>
    </span>
    <span
      class="flex py-3 px-[10px] md:px-[20px] border rounded-[10px] min-w-[120px] md:min-w-[195px] border-transparent justify-center bg-[#12294A]"
    >
      <provider-icon class="mr-3" />
      <span>Providers</span>
    </span>
  </div>
</template>
