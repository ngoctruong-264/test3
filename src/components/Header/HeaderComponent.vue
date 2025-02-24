<script setup>
import MenuIcon from './MenuIcon.vue'
import MainLogo from './MainLogo.vue'
</script>

<template>
  <div
    class="h-[50px] md:h-[67px] flex justify-between border-b-[#03193A66] md:mx-[120px] mx-[20px] mt-[5px]"
  >
    <span class="flex items-center">
      <menu-icon class="mr-4" />
      <main-logo />
      <span
        class="ml-[30px] xl:ml-[50px] text-[14px] text-white w-[400px] xl:w-[450px] hidden justify-between items-center lg:flex"
      >
        <span class="flex justify-between items-center">
          <span class="material-symbols-outlined mr-3"> search </span>
          HOME
        </span>
        <span>GAME</span>
        <span>INFOR</span>
        <span>PROMOTIONS</span>
        <span>VIP</span>
      </span>
    </span>
    <span class="flex items-center text-white">
      <button class="py-[9px] px-[12px] bg-[#12294A] mr-2 rounded-[10px]">LOGIN</button>
      <button class="py-[9px] px-[12px] bg-[#01AF70] rounded-[10px]">REGISTRATION</button>
    </span>
  </div>
</template>
