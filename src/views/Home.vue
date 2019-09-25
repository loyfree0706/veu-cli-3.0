<template lang="pug">
div
  test
</template>

<script>
// @ is an alias to /src

import left_section from '@/components/dev/left_section.vue'
import right_section from '@/components/dev/right_section.vue'
import intro from '@/components/dev/intro.vue'
import box1 from '@/components/test/box1.vue'
import box2 from '@/components/test/box2.vue'
import test from '@/components/test/test.vue'

export default {
  name: 'Home',
  components: {
    left_section,
    right_section,
    intro,
    box1,
    box2,
    test
  }
}
</script>
