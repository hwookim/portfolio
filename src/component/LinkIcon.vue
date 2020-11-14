<template>
  <a
    :href="src"
    target="_blank"
    class="inline-block items-center text-blue-600"
  >
    <span class="content">
      <slot></slot>
    </span>
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

<style scoped lang="scss">
.content {
  .mdi {
    color: black;
  }
}
</style>
