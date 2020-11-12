<template>
  <a :href="src" target="_blank" class="inline-block items-center hover:text-blue-600">
    <slot></slot>
    <i class="mdi mdi-link-variant"></i>
  </a>
</template>

<script>
export default {
  name: 'LinkIcon',
  props: {
    src: {
      type: String,
      required: true,
    },
  },
};
</script>
