<template>
  <div class="flex items-center text-gray-900 py-2">
    <div class="flex-shrink-0">
      <img class="h-12 w-12 rounded-full" :src="email.img" alt="user image" />
    </div>
    <div class="flex-grow px-3">
      <p class="font-semibold text-lg">
        {{ email.subject }}
        <time
          class="text-xs uppercase tracking-wide text-gray-600 sm:hidden"
          datetime="2021-02-20"
        >
          {{ formattedDate }}</time
        >
      </p>
      <span class="flex">
        <span class="text-gray-600 mr-2">me - {{ email.name }}</span>
        <span
          class="px-2 flex items-center bg-emerald-100 text-emerald-900 border border-emerald-500 rounded-full uppercase tracking-wide text-xs font-semibold"
          ><span
            class="h-2 w-2 rounded-full bg-emerald-500 mr-1"
            role="presentation"
          ></span
          >{{ email.tag }}</span
        >
      </span>
    </div>
    <div class="hidden sm:flex">
      <time
        class="text-base font-semibold uppercase tracking-wide text-gray-600"
        datetime="2021-02-20"
      >
        {{ formattedDate }}</time
      >
    </div>
  </div>
</template>

<script setup>
import { computed, defineProps } from "vue";

const props = defineProps({
  email: {
    id: String,
    img: String,
    name: String,
    subject: String,
    date: String,
    tag: String,
  },
});

const formattedDate = computed(() => {
  const date = new Date(props.email.date);
  return date.toLocaleDateString();
});
</script>
