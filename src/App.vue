<template>
  <div id="app">
    <div class="list">
    </div>
    <div class="editor">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app'
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
