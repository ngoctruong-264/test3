<template>
  <div
    class="flex justify-between mx-[20px] md:mx-[50px] 2xl:mx-[240px] max-w-[1440px] items-center text-white my-[20px]"
  >
    <span class="text-[32px] font-semibold">Exclusive Games</span>
    <span class="flex items-center text-[15px] font-normal">
      SEE ALL
      <all-icon class="ml-[10px]" />
    </span>
  </div>
  <div class="flex mx-[20px] md:mx-[50px] 2xl:mx-[240px] overflow-y-auto max-w-[1440px] gap-5">
    <game-item v-for="(game, index) in listGame" :type="game.type" :tag="game.tag" :key="index" />
  </div>
</template>
<script setup>
import AllIcon from '../Providers/Icon/AllIcon.vue'
import GameItem from './GameItem.vue'
const listGame = [
  {
    type: 'VELIPLAY',
    tag: 'new',
  },
  {
    type: 'VELIPLAY',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
  },
  {
    type: 'VELIPLAY',
  },
  {
    type: 'VELIPLAY',
    tag: 'hot',
  },
  {
    type: 'ONLYPLAY',
  },
  {
    type: 'VELIPLAY',
    tag: 'new',
  },
  {
    type: 'VELIPLAY',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
  },
  {
    type: 'VELIPLAY',
    tag: 'new',
  },
  {
    type: 'VELIPLAY',
    tag: 'hot',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
  },
]
</script>
