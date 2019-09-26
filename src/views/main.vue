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



*
  box-sizing: border-box
body
  overflow: hidden

html,
body
  padding: 0
  margin: 0

.main
  display: flex
  overflow: hidden
  height: 100vh
  position: relative
  width: 100%
  backface-visibility: hidden
  will-change: overflow

::-webkit-scrollbar
  display: none
::-moz-selection
  color: #1106CC
  background: #FFFF99
::selection
  color: #1106CC
  background: #FFFF99

.left,
.right
  padding: 0
  margin: 0
  -webkit-overflow-scrolling: touch
  -ms-overflow-style: none
  overflow: auto
  height: auto

@media(min-width: 576px)//表示視窗>576時
  .left,
  .right
    height: 100vh
    width: 100vw

@media(max-width: 575px)//表示視窗<575時
  .left,
  .right
    height: 100vh
    width: 100vw
    display: block

</style>