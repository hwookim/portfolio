<template>
  <div class="flex items-center">
    <div class="w-1/4 md:w-1/5 font-bold">{{ type }}</div>
    <div class="w-3/4 md:w-4/5">
      <div ref="skills" class="hidden">
        <slot></slot>
      </div>
      <skill-box-item v-for="(skill, i) in skills" :key="i">
        {{ skill }}
      </skill-box-item>
    </div>
  </div>
</template>

<script>
import SkillBoxItem from '@/component/SkillBoxItem.vue';

export default {
  name: 'SkillBox',
  components: {
    SkillBoxItem,
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
