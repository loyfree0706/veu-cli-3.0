<template lang="pug">
//- div.row
//-   div.col.col-md-6.col-12.left
//-     left_section
//-   div.col.col-md-6.col-12.right
//-     right_section
div
  div.left
    left_section
  div.right
    right_section
    
</template>

<script>
// @ is an alias to /src

import left_section from '@/components/main/left_section.vue'
import right_section from '@/components/main/right_section.vue'
import intro_section from '@/components/main/intro.vue'

export default {
  name: 'Home',
  components: {
    left_section,
    right_section,
    intro_section
  }
}
</script>

<style lang="sass">
@media(max-width: 575.98px)
  .left
    width: 100%
  .right
    width: 100%
@media(min-width: 576px)
  .left
    width: 50%
  .right
    width: 50%

::-webkit-scrollbar
  display: none

.left
  padding: 0
  margin: 0
.right
  padding: 0
  margin: 0
</style>