<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont icon-fanhui back-icon"></div>
    </div>
    <div class="header-input">
      <span class="iconfont icon-sousuo"></span>
      输入城市/景点/游玩主题
    </div>
    <router-link to="/city">
      <div class="header-right">
        {{this.doubleCity}}
        <span class="iconfont icon-jiantou arrow-icon"></span>
      </div>
    </router-link>
  </div>
</template>

<script>
import { mapState, mapGetters } from 'vuex'

export default {
  name: 'HomeHeader',
  computed: {
    ...mapState(['city']),
    ...mapGetters(['doubleCity'])
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    color: #fff
    line-height: $headerHeight
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
      min-width: 1.04rem
      padding: 0 .1rem
      color: #fff
      text-align: center
      .arrow-icon
        font-size: .24rem
</style>
