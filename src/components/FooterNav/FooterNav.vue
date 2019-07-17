<template>
  <div class="bottom-tab">
    <div class="tab-item" @click="goTo('/home')">
      <span><i class="iconfont icon-icon_home"></i></span>
      <span>首页</span>
    </div>
    <div class="tab-item" @click="goTo('/classify')">
      <span><i class="iconfont icon-iconfl"></i></span>
      <span>分类</span>
    </div>
    <div class="tab-item">
      <span><i class="iconfont icon-icon_home"></i></span>
      <span>识物</span>
    </div>
    <div class="tab-item" @click="goTo('/shop')">
      <span><i class="iconfont icon-gouwuche"></i></span>
      <span>购物车</span>
    </div>
    <div class="tab-item" :class="{on: $route.path==='/profile'}" @click="goTo('/personal')">
      <span><i class="iconfont icon-user"></i></span>
      <span>个人</span>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  methods:{
    goTo(path){
      this.$router.replace(path)
    }
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>
  .bottom-tab
    height 98px
    width 100%
    display flex
    position absolute
    bottom 0
    justify-content space-around
    align-items center
    .tab-item
      display flex
      flex-direction column
      align-items center
      color #666
      font-size 25px
      .on
        color red
      span
        i
          font-size 40px
</style>
