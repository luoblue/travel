<template>
  <div>
    <div class="title">猜你喜欢</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl">
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
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1807/ad/ad574bfe6c9e1ceda3.img.png_200x200_ea7a0734.png',
        title: '成都欢乐谷',
        desc: 'XXXXXXXXXXXXX评论'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1807/ad/ad574bfe6c9e1ceda3.img.png_200x200_ea7a0734.png',
        title: '成都欢乐谷',
        desc: 'XXXXXXXXXXXXX评论'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1807/ad/ad574bfe6c9e1ceda3.img.png_200x200_ea7a0734.png',
        title: '成都欢乐谷',
        desc: 'XXXXXXXXXXXXX评论'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1807/ad/ad574bfe6c9e1ceda3.img.png_200x200_ea7a0734.png',
        title: '成都欢乐谷',
        desc: 'XXXXXXXXXXXXX评论'
      }]
    }
  }
}
</script>

<style scoped lang="stylus">
  @import '~style/mixins.styl'
  .title {
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  }
  .item {
    overflow: hidden
    display: flex
    height: 1.9rem
    .item-img {
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    }
    .item-info {
      flex: 1
      padding: .1rem
      .item-title {
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      }
      .item-desc {
        line-height: .4rem
        color: #ccc
        ellipsis()
      }
      .item-button {
        line-height: .44rem
        margin-top: .16rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
      }
    }
  }
</style>
