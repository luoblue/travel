<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1507/a0/7087c85d439e4.jpg_r_640x214_4cd56a30.jpg',
        title: '成都欢乐谷',
        desc: 'XXXXXXXXXXXXX评论'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1507/a0/7087c85d439e4.jpg_r_640x214_4cd56a30.jpg',
        title: '成都欢乐谷',
        desc: 'XXXXXXXXXXXXX评论'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1507/a0/7087c85d439e4.jpg_r_640x214_4cd56a30.jpg',
        title: '成都欢乐谷',
        desc: 'XXXXXXXXXXXXX评论'
      }, {
        id: '0004',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1507/a0/7087c85d439e4.jpg_r_640x214_4cd56a30.jpg',
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
    .item-img-wrapper {
      .item-img {
        width: 100%
      }
    }
    .item-info {
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
    }
  }
</style>
