<template lang="pug">
div
</template>

<script>
import HelloWorld from './components/HelloWorld';
import left_section from '@/components/main/left_section.vue'
import right_section from '@/components/main/right_section.vue'
import intro_section from '@/components/main/intro_section.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    left_section,
    right_section,
    intro_section
  },
  data: () => ({
    //
  }),
};
</script>

<style lang="stylus">

</style>
