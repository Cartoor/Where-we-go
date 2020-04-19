<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key=item.id>
        <img :src="item.imgUrl" class="item-img">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        title: '重庆当地游 4天自由行',
        desc: '抖音玩法🔥3晚重庆网红民宿+魔幻洪崖洞+8D山城夜景+麻辣地道火锅',
        imgUrl: '//imgs.qunarzz.com/vs_ceph_vs_tts/5af58c1f-794b-48e0-bcdc-31e85acdb0ce.jpg_r_480x320x95_3fa90f4e.jpg'
      },
      {
        id: '0002',
        title: '重庆当地游 4天自由行',
        desc: '抖音玩法🔥3晚重庆网红民宿+魔幻洪崖洞+8D山城夜景+麻辣地道火锅',
        imgUrl: '//imgs.qunarzz.com/vs_ceph_vs_tts/5af58c1f-794b-48e0-bcdc-31e85acdb0ce.jpg_r_480x320x95_3fa90f4e.jpg'
      },
      {
        id: '0003',
        title: '重庆当地游 4天自由行',
        desc: '抖音玩法🔥3晚重庆网红民宿+魔幻洪崖洞+8D山城夜景+麻辣地道火锅',
        imgUrl: '//imgs.qunarzz.com/vs_ceph_vs_tts/5af58c1f-794b-48e0-bcdc-31e85acdb0ce.jpg_r_480x320x95_3fa90f4e.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top .2rem
    line-height .8rem
    background #eee
    text-indent .2rem
  .item
    overflow hidden
    display flex
    height 1.9rem
    .item-img
      width 1.7rem
      height 1.7rem
      padding 0.1rem
    .item-info
      flex: 1
      padding 0.1rem
      min-width 0
      .item-title
        line-height 0.54rem
        font-size 0.32rem
        ellipsis()
      .item-desc
        line-height .4rem
        color #ccc
        ellipsis()
      .item-button
        line-height .44rem
        margin-top .16rem
        background #ff9300
        padding 0 .2rem
        border-radius .06rem
        color #fff
</style>S
