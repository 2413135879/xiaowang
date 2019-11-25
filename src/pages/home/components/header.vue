<template>
    <div class="header">
         <div class="header-left">
             <div class="iconfont">&#xe6ed;</div>
             </div>
         <div class="header-input">
             <span class="iconfont">&#xe70a;</span>
             内容</div>
         <div class="header-right">城市
             <span class="iconfont">&#xe6eb;</span>
         </div>
    </div>
</template>

<script>
export default {
    name : 'HomeHeader'
}
</script>

<style lang='stylus' scoped>
   .header
    display: flex
    line-height: .88rem
    background: #00afc7
    color: #fff
    .header-left
      width: .64rem
      float: left
      .back-icon
        text-align: center
        font-size: .4rem
    .header-input
      flex: 1
      height: .64rem
      line-height: .64rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background: #fff
      border-radius: .1rem
      color: #ccc
    .header-right
      min-width: 1.04rem
      padding: 0 .1rem
      float: right
      text-align: center
      color: #fff
      .arrow-icon
        margin-left: -.04rem
        font-size: .24rem
</style>