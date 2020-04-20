<template>
  <ul class="alphabet-list">
    <li class="alphabet-item"  v-for="(item, key) of cities" :key="key">{{key}}</li>
  </ul>
</template>

<script>
export default {
  name: 'CityAlphabet',
  props: {
    cities: Object
  }
}
</script>

<style lang="stylus">
  @import '~styles/variables.styl'
  .alphabet-list
    display flex
    flex-direction column
    justify-content center
    position absolute
    top 1.58rem
    right 0
    bottom 0
    width .4rem
    .alphabet-item
      line-height .44rem
      text-align center
      color $bgColor
</style>
