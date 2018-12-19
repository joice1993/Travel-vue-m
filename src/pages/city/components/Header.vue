<template>
  <div class="header">
    城市选择
    <router-link to="/">
      <div class="iconfont icon-fanhui header-back"></div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
  @import "~styles/varibles.styl"
  .header
    position: relative
    height: $headerHeight
    color: #fff
    font-size: .32rem
    line-height: $headerHeight
    text-align: center
    background: $bgColor
    overflow: hidden
    .header-back
      position: absolute
      top: 0
      left: 0
      width: .64rem
      color: #fff
      font-size: .4rem
      text-align: center
</style>
