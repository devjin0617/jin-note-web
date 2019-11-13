<template>
  <div>
    <ul>
      <note-list-item v-for="i in 20" :key="i"></note-list-item>
    </ul>
  </div>
</template>

<script>
import ListItem from './ListItem'
;
export default {
  name: 'note-list',
  created() {

  },
  components: {
    'note-list-item': ListItem,
  },
};
</script>

<style scoped>
ul {
  list-style-type: none;
  padding: 0;
  margin: 0;
}
</style>
