<template>

<!-- primary color of the project is lightgreen -->

  <h1>lekce 24</h1>
  <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam tempora maiores perferendis molestias asperiores quidem ut explicabo aspernatur, iste maxime assumenda sint amet voluptas repellendus voluptatum quae consectetur eius necessitatibus.</p>
  <TButton label="click me!" />
</template>

<script>

import TButton from '@/components/TButton.vue'
export default {
  name: 'App',
  components: { TButton }
}

</script>

<style lang="stylus" scoped>
@import './styles/variables.styl'
h1
  border-bottom: 2px solid $primary
  margin-bottom: 1rem

</style>