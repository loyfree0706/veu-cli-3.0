<template lang="pug">
div
  p hello
  div.header
    div.title {{title}}
    div.fans
  
  div.content

  div.message

  div.footer  
</template>

<script>
export default {
  data: function () {
    return {
      title:'this is title',
    }
  }
}
</script>

<style lang="sass">
</style>