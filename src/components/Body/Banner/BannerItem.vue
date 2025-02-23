<template>
  <div class="hidden duration-700 ease-in-out" :data-carousel-item="props.active ? 'active' : ''">
    <div
      class="h-[425px] text-white bg-linear-to-r from-[#147261] to-[#082C25] justify-end relative gap-y-5 rounded-[10px] mx-[20px] flex"
    >
      <img
        src="/Image1.png"
        class="lg:hidden absolute right-[20%] top-[-70px] lg:top-0 lg:right-[5px] w-[350px] h-auto md:w-[1/2] xl:w-auto lg:h-full z-[9999]"
        alt="..."
      />
      <span class="text-center lg:max-w-1/2 lg:mt-[80px] mt-[210px]">
        <div class="lg:text-[21px] text-[12px]">
          <span class="py-[6px] px-[16px] bg-[#FFFFFF1A] rounded-[20px]">Exclusive Tournament</span>
        </div>
        <div class="md:text-[42px] text-[24px] md:font-extrabold lg:mt-[20px]">
          Piggy Christmas Tap: €35,000 For Your Wins
        </div>
        <button
          class="text-[15px] mt-[5px] lg:mt-[20px] py-[10px] lg:pt-[16px] lg:pb-[12px] px-[40px] lg:px-[80px] bg-[#FF0960] rounded-[10px]"
        >
          JOIN AND WIN
        </button>
      </span>
      <img
        src="/Image1.png"
        class="hidden lg:block lg:top-0 lg:right-[5px] w-[350px] h-auto md:w-[1/2] xl:w-auto lg:h-full z-[9999]"
        alt="..."
      />
    </div>
  </div>
</template>
<script setup>
const props = defineProps({
  active: {
    type: Boolean,
  },
})
</script>
