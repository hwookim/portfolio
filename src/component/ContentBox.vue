<template>
  <div class="flex w-full flex-col my-2 px-5 md:px-10 py-5 bg-white rounded-xl">
    <div v-if="title" class="ml-5 mb-3 text-2xl font-bold">
      {{ title }}
    </div>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'ContentBox',
  props: {
    title: {
      type: String,
      required: false,
    },
  },
};
</script>
