<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item in recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl" />
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
  name: "HomeRecommend",
  data() {
    return {
      recommendList: [
        {
          id: "0001",
          imgUrl:
            "https://img1.qunarzz.com/travel/poi/1804/f8/654d1576a7497d37.jpg",
          title: "巴拉望（公主港 爱妮岛 科隆岛)",
          desc: "自驾游防城港，广西小众地方也有绝美的风景"
        },
        {
          id: "0002",
          imgUrl:
            "https://img1.qunarzz.com/travel/poi/1804/f8/654d1576a7497d37.jpg",
          title: "巴拉望（公主港 爱妮岛 科隆岛)",
          desc: "自驾游防城港，广西小众地方也有绝美的风景"
        },
        {
          id: "0003",
          imgUrl:
            "https://img1.qunarzz.com/travel/poi/1804/f8/654d1576a7497d37.jpg",
          title: "巴拉望（公主港 爱妮岛 科隆岛)",
          desc: "自驾游防城港，广西小众地方也有绝美的风景"
        },
        {
          id: "0004",
          imgUrl:
            "https://img1.qunarzz.com/travel/poi/1804/f8/654d1576a7497d37.jpg",
          title: "巴拉望（公主港 爱妮岛 科隆岛)",
          desc: "自驾游防城港，广西小众地方也有绝美的风景"
        }
      ]
    };
  }
};
</script>
<style lang='stylus' scope>
@import '~styles/mixins.styl';

.recommend-title {
  margin-top: 0.2rem;
  background: #eeeeee;
  line-height: 0.8rem;
  text-indent: 0.2rem;
}

.item {
  overflow: hidden;
  display: flex;
  height: 1.9rem;
}

.item-img {
  width: 1.7rem;
  height: 1.7rem;
  padding: 0.1rem;
}

.item-info {
  flex: 1;
  padding: 0.1rem;
  min-width: 0;
}

.item-title {
  line-height: 0.54rem;
  font-size: 0.32rem;
}

.item-desc {
  line-height: 0.4rem;
  color: #ccc;
  ellipsis();
}

.item-button {
  line-height: 0.38rem;
  background: #ff9300;
  padding: 0 0.16rem;
  color: #ffffff;
  margin-top: 0.3
  rem;
  border-radius: 0.08rem;
  ellipsis();
}
</style>