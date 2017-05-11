<template>
  <div id="app">
    <note-list class="list"></note-list>
    <div class="editor">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import List from './components/List'

export default {
  name: 'app',
  components: {
    'note-list': List
  }
}
</script>

<style lang='scss'>
#app {
  display: flex;
  height:100vh;

  > div {
    border:1px solid #b5b5b5;
  }

  .list {
    flex:1
  }

  .editor {
    flex:2
  }
}
</style>
