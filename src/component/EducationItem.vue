<template>
  <div class="flex flex-row md:w-1/2 mb-3 items-center">
    <div class="w-12 h-12 mr-3">
      <slot></slot>
    </div>
    <div class="flex flex-col mb-1">
      <a :href="src" target="_blank" class="flex items-center">
        <div class="text-xl font-bold mr-1">{{ name }}</div>
        <i class="mdi mdi-link-variant"></i>
      </a>
      <div class="text-gray-600">{{ period }}</div>
      <div>{{ description }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'EducationItem',
  props: {
    src: {
      type: String,
      required: true,
    },
    name: {
      type: String,
      required: true,
    },
    period: {
      type: String,
      required: true,
    },
    description: {
      type: String,
    },
  },
};
</script>
