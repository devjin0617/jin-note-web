<template>
  <div id="app">
    <div class="navibar">
      <span>JIN NOTE</span>
    </div>
    <div class="main">
      <note-list class="list"></note-list>
      <div class="editor">
        <router-view></router-view>
      </div>
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
  flex-direction:column;

  .navibar {
    width:100%;
    height:40px;
    background-color:#333333;
    color:white;
    display:flex;
    align-items:center;
    justify-content:center;
  }

  .main {
    border:1px solid #b5b5b5;
    flex:1;
    display:flex;
  }

  .list {
    flex:1;
    overflow:scroll;
  }

  .editor {
    flex:2
  }
}
</style>
