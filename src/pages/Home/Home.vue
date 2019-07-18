<template>
  <section id="home">
    <Header class="header">
      <span class="header-left"><a href="">网易严选</a></span>
      <span class="header-input">
        <i class="iconfont icon-iconset0157"></i>
        <input class="header-text" type="text" placeholder="搜索~~~~~~~">
      </span>
      <span class="header-right">
        <span class="header-login">登录</span>
      </span>
    </div>
  </Header>
  <nav class="-container">
    <div class="swiper-container">
    <div class="swiper-wrapper">
        <div class="swiper-slide"><img src="https://yanxuan.nosdn.127.net/5d8d67832db5757f2941c3cfe0ffd558.jpg?imageView&quality=75&thumbnail=750x0" alt=""></div>
        <div class="swiper-slide"><img src="https://yanxuan.nosdn.127.net/3cf97a99f8017e3bb0d22fdff2c283b0.jpg?imageView&quality=75&thumbnail=750x0" alt=""></div>
        <div class="swiper-slide"><img src="https://yanxuan.nosdn.127.net/e1838f8442e7bfef014070ff902a698f.jpg?imageView&quality=75&thumbnail=750x0" alt=""></div>
    </div>
    <div class="swiper-pagination"></div>
</div>
  </nav>
  </section>
</template>

<script type="text/ecmascript-6">
  import Swiper from 'swiper'
  import "swiper/dist/css/swiper.css"

  export default {
    mounted () {
      var mySwiper = new Swiper ('.swiper-container', {
    //direction: 'vertical', // 垂直切换选项
    loop: true, // 循环模式选项
      // 如果需要分页器
      pagination: {
        el: '.swiper-pagination',
      }
      })
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>
  @import '../../common/stylus/mixins.styl'
  #home
    width 100%
    .header
      width 100%
      height 44px
      display flex
      align-items center
      justify-content space-around
      .header-left
        a
          text-decoration none
          font-weight bold
          color block
      .header-input
        .iconfont
          position absolute
          margin  7px 14px
        .header-text
          height 28px
          width 221px
          border-radius 8px
          color #666
          background-color #ededed
          border 1px solid #eee
          text-align center
      .header-login
        color #f40
        width 35px
        height 19px
        border 1px solid
        padding 5px
        border-radius 5px
        font-size 14px
</style>
