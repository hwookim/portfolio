<template>
  <div class="flex w-full flex-col my-2 px-5 md:px-10 py-5 bg-white rounded-xl">
    <div v-if="title" class="flex mb-5 items-center">
      <div class="w-auto mx-5 text-2xl font-bold">
        {{ title }}
      </div>
      <div class="flex-auto border-t-8 border-blue-800"></div>
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
