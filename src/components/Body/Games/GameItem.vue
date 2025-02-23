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
})
</script>
<template>
  <span class="md:min-w-[156px] min-w-[120px] relative">
    <img src="/game1.png" alt="" class="rounded-[10px]" />
    <span class="absolute bottom-0 right-[50%] text-white font-medium">{{ props.type }}</span>
    <hot-tag class="absolute top-[15px]" v-if="props.tag === 'hot'" />
    <new-tag class="absolute top-[15px]" v-if="props.tag === 'new'" />
  </span>
</template>
