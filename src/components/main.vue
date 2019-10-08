<template>
  <div class="mainInfo">
    <div class="header">
      <span>首页</span>
      <span>关于我们</span>
    </div>
    <div class="content">
      <img src="../assets/background.png" alt="" />
    </div>
    <div class="footer">
      随人科技 版权所有 2008-2020 苏ICP备15007261号-1
    </div>
  </div>
</template>

<script>
export default {
  name: 'mainInfo',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.mainInfo {
  position: relative;
  .header {
    position: absolute;
    top: 2%;
    right: 5%;
    width: 20%;
    span {
      margin-right: 10%;
    }
  }
  .content {
    width: 100%;
    background-size: cover;
    img {
      background-size: contain;
      width: 100%;
      height: auto;
    }
  }
  .footer {
    position: absolute;
    bottom: 3%;
    width: 100%;
    text-align: center;
  }
}
</style>