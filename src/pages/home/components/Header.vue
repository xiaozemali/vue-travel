<template>
  <div class="header">
    <div class="header-left">
    <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
    <span class="iconfont">&#xe632;</span>
    输入城市/景点/游玩主题</div>
    <div class="header-right">
    城市
    <span class="iconfont">&#xe62d;</span>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style lang='stylus' scope>
@import '~styles/varibles.styl';

.header {
  display: flex;
  line-height: 0.86rem;
  background: $bgColor;
  color: #fff;

  .header-left {
    width: 0.64rem;
    float: left;

    .back-icon{
        text-align :center;
        font-size :.4rem
    }
  }

  .header-input {
    flex: 1;
    height: 0.64rem;
    line-height: 0.64rem;
    background: #ffffff;
    border-radius: 0.1rem;
    margin-top: 0.12rem;
    margin-left: 0.2rem;
    color: #ccc;
    padding-left .2rem;
  }

  .header-right {
    width: 1.24rem;
    float: right;
    text-align: center;
  }
}
</style>