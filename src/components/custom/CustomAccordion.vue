<template>
  <div :id="props.id" class="mb-2">
    <h2 :id="`${props.id}-heading-1`" class="w-full">
      <button
        type="button"
        class="flex items-center justify-between w-full p-2 font-medium rtl:text-right text-white bg-[#1A3157] rounded-[10px] focus:ring-4 dark:border-gray-700 dark:text-gray-400"
        :data-accordion-target="`#${props.id}-body-1`"
        :aria-controls="`${props.id}-body-1`"
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
    <div :id="`${props.id}-body-1`" class="hidden" :aria-labelledby="`${props.id}-heading-1`">
      <div class="p-4">
        <ul>
          <li v-for="(item, idx) in props.section" :key="idx" class="p-1">
            {{ item }}
          </li>
        </ul>
      </div>
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
