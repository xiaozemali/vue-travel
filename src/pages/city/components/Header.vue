<template>
  <div class="header">
    城市选择
    <router-link to="/">
      <div class="iconfont header-back">&#xe624;</div>
    </router-link>
  </div>
</template>
<script>
export default {
  name: "CityHeader"
};
</script>
<style lang='stylus' scope>
@import '~styles/varibles.styl';

.header {
  position: relative;
  height: $headerHeight;
  overflow: hidden;
  line-height: $headerHeight;
  text-align: center;
  color: #ffffff;
  background: $bgColor;
  font-size: 0.32rem;

  .header-back {
    position: absolute;
    width: 0.64rem;
    text-align: center;
    font-size: 0.4rem;
    left: 0;
    top: 0;
    color: #ffffff;
  }
}
</style>