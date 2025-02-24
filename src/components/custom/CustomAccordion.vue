<template>
  <h2 :id="`accordion-collapse-heading-${props.id}`" class="w-full">
    <button
      type="button"
      class="flex items-center justify-between w-full p-2 font-medium rtl:text-right text-white focus:bg-[#1A3157] bg-[#1A3157] rounded-[10px] mb-3"
      :data-accordion-target="`#accordion-collapse-body-${props.id}`"
      aria-expanded="false"
      :aria-controls="`accordion-collapse-body-${props.id}`"
    >
      <span>{{ props.title }}</span>
      <svg
        data-accordion-icon
        class="w-3 h-3 rotate-180 shrink-0"
        aria-hidden="true"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 10 6"
      >
        <path
          stroke="currentColor"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M9 5 5 1 1 5"
        />
      </svg>
    </button>
  </h2>
  <div
    :id="`accordion-collapse-body-${props.id}`"
    class="hidden"
    :aria-labelledby="`accordion-collapse-heading-${props.id}`"
  >
    <div class="p-4 pt-0">
      <ul>
        <li v-for="(item, idx) in props.section" :key="idx" class="p-1">
          {{ item }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  id: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  section: {
    type: Array,
    required: true,
  },
})
</script>
