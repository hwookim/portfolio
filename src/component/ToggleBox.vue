<template>
  <div class="mb-3">
    <div class="flex font-bold" @click="toggle">
      <div class="mr-2">{{ mark }}</div>
      <slot name="title"></slot>
    </div>
    <div class="p-5 bg-gray-100" :class="{ hidden }">
      <slot name="content"></slot>
    </div>
  </div>
</template>

<script>
const NOT_OPENED = '▶︎';
const OPENED = '▼';

export default {
  name: 'ToggleBox',
  data() {
    return {
      mark: NOT_OPENED,
      hidden: true,
    };
  },
  methods: {
    toggle() {
      this.mark = this.mark === NOT_OPENED ? OPENED : NOT_OPENED;
      this.hidden = !this.hidden;
    },
  },
};
</script>
