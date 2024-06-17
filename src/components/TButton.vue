<template>
  <button @click="$emit('clicked')">{{ label }}</button>
</template>

<script>

export default {
  name: 'TButton',
  props: {
    label: String
  }
}

</script>
<style lang="stylus" scoped>
@import '../styles/variables.styl'

button
  font-size: 1.4rem
  padding: .4em .8em
  border-radius: 5px
  border: 2px solid #222
  if dark($primary)
    color: white
  else
    color: #222
  background: $primary
  cursor: pointer
  transition: background-color .4s ease
  &:hover
    if dark($primary)
      background: darken($primary, 40%)
    else
      background: lighten($primary, 40%)

</style>