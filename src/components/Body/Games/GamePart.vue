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
    <game-item
      v-for="(game, index) in listGame"
      :type="game.type"
      :tag="game.tag"
      :key="index"
      :srcImg="game.srcImg"
    />
  </div>
</template>
<script setup>
import AllIcon from '../Providers/Icon/AllIcon.vue'
import GameItem from './GameItem.vue'
const listGame = [
  {
    type: 'VELIPLAY',
    tag: 'new',
    srcImg: '/game1.png',
  },
  {
    type: 'VELIPLAY',
    srcImg: '/game1.png',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
    srcImg: '/game2.png',
  },
  {
    type: 'VELIPLAY',
    srcImg: '/game3.png',
  },
  {
    type: 'VELIPLAY',
    tag: 'hot',
    srcImg: '/game2.png',
  },
  {
    type: 'ONLYPLAY',
    srcImg: '/game3.png',
  },
  {
    type: 'VELIPLAY',
    tag: 'new',
    srcImg: '/game3.png',
  },
  {
    type: 'VELIPLAY',
    srcImg: '/game2.png',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
    srcImg: '/game2.png',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
    srcImg: '/game3.png',
  },
  {
    type: 'VELIPLAY',
    tag: 'new',
    srcImg: '/game2.png',
  },
  {
    type: 'VELIPLAY',
    tag: 'hot',
    srcImg: '/game3.png',
  },
  {
    type: 'ONLYPLAY',
    tag: 'new',
    srcImg: '/game1.png',
  },
]
</script>
