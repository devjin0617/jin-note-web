<template>
  <div>
    <ul>
      <note-list-item v-for="i in 10"></note-list-item>
    </ul>
  </div>
</template>

<script>
import ListItem from './ListItem'
export default {
  name: 'note-list',
  created () {

  },
  components: {
    'note-list-item': ListItem
  }
}
</script>

<style>
</style>
