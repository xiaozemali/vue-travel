<template>
  <div>
    <div class="recommend-title">周末去哪</div>
    <ul>
      <li class="item, border-bottom" v-for="item in list" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" />
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
  name: "HomeWeekend",
  props:{
    list:Array
  }
};
</script>
<style lang='stylus' scoped>
@import '~styles/mixins.styl';

.recommend-title {
  margin-top: 0.2rem;
  background: #eeeeee;
  line-height: 0.8rem;
  text-indent: 0.2rem;
}

.item {
  overflow: hidden;
  height: 1.9rem;
}

.item-img-wrapper {
  overflow: hidden;
  padding-bottom: 23.98%;
  height: 0;
}

.item-img {
  width: 100%;
}

.item-info {
  padding: 0.2rem;
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


</style>