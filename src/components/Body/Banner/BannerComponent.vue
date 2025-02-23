<template>
  <div id="indicators-carousel" class="mx-[10%] overflow-hidden" data-carousel="static">
    <!-- Carousel wrapper -->
    <div class="md:h-96 relative">
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
    <div
      class="absolute z-30 flex -translate-x-1/2 space-x-3 rtl:space-x-reverse bottom-[180px] left-1/2"
    >
      <button
        type="button"
        class="w-3 h-3 rounded-full"
        aria-current="true"
        aria-label="Slide 1"
        data-carousel-slide-to="0"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full"
        aria-current="false"
        aria-label="Slide 2"
        data-carousel-slide-to="1"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full"
        aria-current="false"
        aria-label="Slide 3"
        data-carousel-slide-to="2"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full"
        aria-current="false"
        aria-label="Slide 4"
        data-carousel-slide-to="3"
      ></button>
      <button
        type="button"
        class="w-3 h-3 rounded-full"
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
