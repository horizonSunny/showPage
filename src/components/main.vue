<template>
  <div class="mainInfo">
    <div class="header">
      <span @click="clickhome">首页</span>
      <span @click="clickConcat">关于我们</span>
    </div>
    <div class="content">
      <img v-if="homeInfo" src="../assets/background.png" alt="" />
      <img v-if="!homeInfo" src="../assets/guanyu.png" alt="" />
    </div>
    <div class="footer">
      燧人科技 版权所有 2008-2020 沪ICP备11000614号-4
    </div>
  </div>
</template>

<script>
export default {
  name: 'mainInfo',
  data () {
    return {
      homeInfo: true
    }
  },
  methods: {
    clickhome () {
      this.homeInfo = true
    },
    clickConcat () {
      this.homeInfo = false
    }
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