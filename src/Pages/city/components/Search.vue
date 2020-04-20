<template>
  <div class="search">
    <input type="text" class="search-input" placeholder="输入城市名或拼音">
  </div>
</template>

<script>
export default {
  name: 'CitySearch'
}
</script>

<style lang="stylus">
  @import '~styles/variables.styl'
  .search
    background $bgColor
    height .72rem
    padding 0 .1rem
    .search-input
      box-sizing border-box
      width 100%
      padding 0 .1rem
      height .62rem
      line-height .62rem
      text-align center
      border-radius .06rem
</style>
