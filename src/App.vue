<script setup>
import HeaderComponent from './components/Header/HeaderComponent.vue'
import FooterComponent from './components/Footer/FooterComponent.vue'
import BannerComponent from './components/Body/Banner/BannerComponent.vue'
import FilterComponent from './components/Body/Filter/FilterComponent.vue'
import GamePart from './components/Body/Games/GamePart.vue'
import ProviderPart from './components/Body/Providers/ProviderPart.vue'
</script>

<template>
  <header-component />

  <div class="pt-[67px] overflow-hidden">
    <banner-component />
    <filter-component />
    <game-part />
    <provider-part />
  </div>
  <footer-component />
</template>

<style scoped>
.logo {
  display: block;
}
</style>
