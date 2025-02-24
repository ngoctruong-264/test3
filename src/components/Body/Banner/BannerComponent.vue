<template>
  <div id="indicators-carousel relative text-center" class="mx-[10%]" data-carousel="static">
    <!-- Carousel wrapper -->
    <div class="h-[350px] lg:h-96 relative">
      <!-- Item 1 -->
      <banner-item :active="true" />
      <!-- Item 2 -->
      <banner-item />
      <!-- Item 3 -->
      <banner-item />
      <!-- Item 4 -->
      <banner-item />
      <!-- Item 5 -->
      <banner-item />
    </div>
    <!-- Slider indicators -->
    <div class="z-30 mt-[10px] md:mt-[50px] mb-[20px] text-center gap-5">
      <button
        type="button"
        class="w-3 h-3 rounded-full mx-1"
        aria-current="true"
        aria-label="Slide 1"
        data-carousel-slide-to="0"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full mx-1"
        aria-current="false"
        aria-label="Slide 2"
        data-carousel-slide-to="1"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full mx-1"
        aria-current="false"
        aria-label="Slide 3"
        data-carousel-slide-to="2"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full mx-1"
        aria-current="false"
        aria-label="Slide 4"
        data-carousel-slide-to="3"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full mx-1"
        aria-current="false"
        aria-label="Slide 5"
        data-carousel-slide-to="4"
      ></button>
    </div>
  </div>
</template>
<script setup>
import BannerItem from './BannerItem.vue'
</script>
