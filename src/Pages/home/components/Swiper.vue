<template>
  <div class="wrapper">
    <swiper :options="swiperOptions">
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" alt="">
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOptions: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        imgUrl: '//m.360buyimg.com/mobilecms/s700x280_jfs/t1/102456/23/17079/182726/5e854aedE239daed9/f7d9b843807e08ed.jpg!cr_1125x445_0_171!q70.jpg.dpg',
        id: '0001'
      }, {
        imgUrl: '//m.360buyimg.com/mobilecms/s700x280_jfs/t1/108908/10/11124/142233/5e85a443E85577f00/bbe190fd93ce5fbc.jpg!cr_1125x445_0_171!q70.jpg.dpg',
        id: '0002'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background-color #fff !important
  .wrapper
    overflow hidden
    width 100%
    height 0
    padding-bottom 39.57%
  .swiper-img
    width 100%
</style>
