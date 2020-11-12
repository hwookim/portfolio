<template>
  <div class="flex">
    <div class="w-1/4 md:w-1/5 font-bold">{{ type }}</div>
    <div class="w-3/4 md:w-4/5">
      <div ref="skills" class="hidden">
        <slot></slot>
      </div>
      <skill-item v-for="(skill, i) in skills" :key="i">{{ skill }}</skill-item>
    </div>
  </div>
</template>

<script>
import SkillItem from '@/component/SkillItem.vue';

export default {
  name: 'SkillBox',
  components: {
    SkillItem,
  },
  props: {
    type: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      skills: [],
    };
  },
  mounted() {
    const skills = this.$refs.skills.innerText;
    this.skills = skills.split(', ');
  },
};
</script>
