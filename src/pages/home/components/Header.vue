<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont icon-fanhui back-icon"></div>
    </div>
    <div class="header-input">
      <span class="iconfont icon-sousuo"></span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      {{this.city}}
      <span class="iconfont icon-jiantou arrow-icon"></span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    color: #fff
    line-height: .86rem
    background: $bgColor
    .header-left
      float: left
      width: .64rem
      .back-icon
        text-align: center
        font-size: .35rem
    .header-input
      flex: 1
      height: .64rem
      line-height: .64rem
      margin: .12rem 0 0 .2rem
      padding-left: .2rem
      color: #ccc
      background: #fff
      border-radius: .1rem
    .header-right
      float: right
      width: 1.24rem
      text-align: center
      .arrow-icon
        font-size: .24rem
</style>
