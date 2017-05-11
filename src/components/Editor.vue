<template>
  <div>
    <textarea id="note-editor">{{text}}</textarea>
  </div>
</template>

<script>

export default {
  name: 'note-editor',
  data () {
    return {
      text: ''
    }
  },
  created () {

  },
  mounted () {
    const options = {
      element: document.getElementById('note-editor'),
      toolbar: ['bold', 'italic', 'heading', '|', 'code', 'quote', '|', 'unordered-list', 'ordered-list', '|', 'clean-block', '|', 'link', 'image', 'table', '|', 'preview'],
      placeholder: '여기에 글을 작성해주세요'
    }
    let simplemde = new this.SimpleMDE(options)
    simplemde.value('')
  }
}
</script>

<style lang="scss">
.editor {
  > div {
    height: 100%;
    display: flex;
    flex-direction: column;

    .CodeMirror {
      flex:1;
    }
  }
}
</style>
