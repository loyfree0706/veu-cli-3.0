<template lang="pug">
div.main
  div.intro
    intro_section
  div.left
    left_section
  div.right
    right_section
    
</template>

<script>
// @ is an alias to /src

import left_section from '@/components/main/left_section.vue'
import right_section from '@/components/main/right_section.vue'
import intro_section from '@/components/main/intro_section.vue'

export default {
  name: 'main',
  components: {
    left_section,
    right_section,
    intro_section
  }
}
</script>

<style lang="sass">
@media(max-width: 575.98px)
  .left,
  .right
    width: 100%

@media(min-width: 576px)
  .left,
  .right
    width: 50%

::-webkit-scrollbar
  display: none

.left,
.right
  padding: 0
  margin: 0
  -webkit-overflow-scrolling: touch
  -ms-overflow-style: none
  overflow: auto
  height: auto
  padding: .5rem

*
  box-sizing: border-box
body
  overflow-x: hidden

html,
body
  padding: 0
  margin: 0
  color: #ebebeb

.main
    display: flex
    overflow: hidden
    height: 100vh
    position: relative
    width: 100%
    backface-visibility: hidden
    will-change: overflow

</style>