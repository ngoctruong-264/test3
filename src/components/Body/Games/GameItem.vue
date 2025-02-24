<script setup>
import HotTag from './HotTag.vue'
import NewTag from './NewTag.vue'
const props = defineProps({
  tag: {
    type: String,
  },
  type: {
    type: String,
    required: true,
  },
  srcImg: {
    type: String,
    required: true,
  },
})
</script>
<template>
  <span class="md:min-w-[156px] min-w-[120px] relative">
    <img :src="props.srcImg" alt="" class="rounded-[10px]" />
    <span class="absolute bottom-0 text-white font-medium w-full text-center text-[8px]">{{
      props.type
    }}</span>
    <hot-tag class="absolute top-[15px]" v-if="props.tag === 'hot'" />
    <new-tag class="absolute top-[15px]" v-if="props.tag === 'new'" />
  </span>
</template>
