<template>
  <div class="about">
    <van-field v-model="value" label="淦" placeholder="淦淦淦淦淦淦" />
    <van-swipe class="index_swipe" :autoplay="3000" indicator-color="white">
      <van-swipe-item><img src="http://sky.hongzhiyu.top/static/hwj.png"><img src="http://sky.hongzhiyu.top/static/hwj.png"></van-swipe-item>
      <van-swipe-item><img src="http://sky.hongzhiyu.top/static/hhc.png"><img src="http://sky.hongzhiyu.top/static/hhc.png"></van-swipe-item>
      <van-swipe-item><img src="http://sky.hongzhiyu.top/static/jnq.png"><img src="http://sky.hongzhiyu.top/static/jnq.png"></van-swipe-item>
      <van-swipe-item><img src="http://sky.hongzhiyu.top/static/ymz.png"><img src="http://sky.hongzhiyu.top/static/ymz.png"></van-swipe-item>
      <van-swipe-item><img src="http://sky.hongzhiyu.top/static/xpf.png"><img src="http://sky.hongzhiyu.top/static/xpf.png"></van-swipe-item>
    </van-swipe>
    <van-row class="index_desc">
      <van-col span="8">淦</van-col>
      <van-col span="8">淦</van-col>
      <van-col span="8">淦</van-col>
    </van-row>
    <div class="index_banner01">
      <img src="http://static.fcbox.com/fcapp/mall/202104/zqob4pcubqa.gif" />
    </div>
    <van-grid :column-num="5" class="index_nav">
      <van-grid-item
        v-for="value in 10"
        :key="value"
        icon="photo-o"
        text="淦"
      />
    </van-grid>
    <div class="index_banner02">
      <img src="http://static.fcbox.com/fcapp/mall/202104/wjng7ip6ezr.jpg" />
    </div>
    <div class="index_down">
      <div class="title">
        <span class="left">限时直降</span>
        <span class="right">更多 ></span>
      </div>
      <ul class="content">
        <li class="item">淦</li>
        <li class="item">淦</li>
        <li class="item">淦</li>
        <li class="item">淦</li>
        <li class="item">淦</li>
        <li class="item">淦</li>
      </ul>
    </div>
    <van-row class="index_banner03" gutter="20">
      <van-col span="12"
        ><img src="http://static.fcbox.com/fcapp/mall/202104/1398e6rf9jj.png"
      /></van-col>
      <van-col span="12"
        ><img src="http://static.fcbox.com/fcapp/mall/202104/opvu77w4o5.png"
      /></van-col>
    </van-row>
    <ul class="index_pro">
      <li v-for="img in imageList" :key="img">
        <img v-lazy="img" />
      </li>
    </ul>
    <van-tabbar v-model="active">
      <van-tabbar-item icon="home-o">淦</van-tabbar-item>
      <van-tabbar-item icon="search">淦</van-tabbar-item>
      <van-tabbar-item icon="friends-o">淦</van-tabbar-item>
      <van-tabbar-item icon="setting-o">淦</van-tabbar-item>
    </van-tabbar>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      value: "",
       active: 0,
      imageList: [
        "https://img01.yzcdn.cn/vant/apple-1.jpg",
        "https://img01.yzcdn.cn/vant/apple-2.jpg",
        "http://static.fcbox.com/fcapp/mall/bh8oa4awgx9.jpg",
        "http://static.fcbox.com/fcapp/mall/mff9mg228l.jpg",
        "http://static.fcbox.com/fcapp/mall/tamt6w8vn3q.jpg",
        "https://img01.yzcdn.cn/vant/apple-1.jpg",
        "https://img01.yzcdn.cn/vant/apple-2.jpg",
        "http://static.fcbox.com/fcapp/mall/bh8oa4awgx9.jpg",
        "http://static.fcbox.com/fcapp/mall/mff9mg228l.jpg",
        "http://static.fcbox.com/fcapp/mall/tamt6w8vn3q.jpg",
        "https://img01.yzcdn.cn/vant/apple-1.jpg",
        "https://img01.yzcdn.cn/vant/apple-2.jpg",
        "http://static.fcbox.com/fcapp/mall/bh8oa4awgx9.jpg",
        "http://static.fcbox.com/fcapp/mall/mff9mg228l.jpg",
        "http://static.fcbox.com/fcapp/mall/tamt6w8vn3q.jpg",
        "https://img01.yzcdn.cn/vant/apple-1.jpg",
        "https://img01.yzcdn.cn/vant/apple-2.jpg",
        "http://static.fcbox.com/fcapp/mall/bh8oa4awgx9.jpg",
        "http://static.fcbox.com/fcapp/mall/mff9mg228l.jpg",
        "http://static.fcbox.com/fcapp/mall/tamt6w8vn3q.jpg",
      ],
    };
  },
  created() {},
  mounted() {},
  methods: {},
  computed: {},
  watch: {},
  destroyed() {},
};
</script>
<style lang="less" scoped>
//@import url(); 引入公共css类
.about {
  min-height: 100%;
  background: #f6f6f6;
  padding: 10px;
  padding-bottom: 60px;
  box-shadow: 0px 1px 4px 0px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  .index_swipe {
    font-size: 66px;
    .van-swipe-item {
      color: #fff;
      text-align: center;
      background-color: #eee;
      display: flex;
      justify-content: space-around;
      img{
        width: 150px;
        height: 150px;
      }
    }
  }
  .index_desc {
    margin-top: 5px;
    background-color: #fff;
    .van-col {
      height: 40px;
      line-height: 40px;
      border: 1px solid #eee;
    }
  }
  .index_banner01 {
    margin-top: 5px;
  }
  .index_nav {
    margin-top: 5px;
  }
  .index_banner02 {
    margin-top: 5px;
    height: 126px;
  }
  .index_down {
    margin-top: 5px;
    .title {
      display: flex;
      height: 34px;
      line-height: 34px;
      .left {
        font-size: 18px;
        font-weight: 700;
        flex: 1;
        text-align: left;
      }
      .right {
        flex: 1;
        text-align: right;
      }
    }
    .content {
      font-size: 40px;
      overflow: auto;
      white-space: nowrap;
      .item {
        height: 143px;
        line-height: 143px;
        width: 100px;
        display: inline-block;
      }
    }
  }
  .index_banner03 {
    margin-top: 5px;
    .van-col {
      height: 104px;
      line-height: 104px;
      img {
        border-radius: 15px;
      }
    }
  }
  .index_pro {
    margin-top: 5px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    li {
      width: 48%;
    }
  }
}
</style>
