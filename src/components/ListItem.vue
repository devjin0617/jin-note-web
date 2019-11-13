<template>
  <li class="list-item">
    <div class="title">제목입니다</div>
    <div class="content">
      내용입니다
    </div>
  </li>
</template>

<script>
export default {
  name: 'note-list-item',
  created() {

  },
};
</script>

<style scoped lang='scss'>
.list-item {
  width:100%;
  height:80px;
  border-bottom:1px solid #b5b5b5;
  display: flex;
  flex-direction: column;
  padding:5px;

  > div {
    width:100%;
    word-break: break-all;
    overflow: hidden;
  }

  .title {
    height:20px;
    font-weight:bold;
  }

  .content {
    margin-top:5px;
    flex: 1;
  }
}
</style>
