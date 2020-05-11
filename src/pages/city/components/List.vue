<template>
  <div class="list">
    <div class="area">
      <div class="title border-topbottom">当前城市</div>
      <div class="button-list">
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
      </div>
    </div>
    <div class="area">
      <div class="title border-topbottom">热门城市</div>
      <div class="button-list">
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
        <div class="button-wrapper">
          <div class="button">北京</div>
        </div>
      </div>
    </div>
    <div class="area">
      <div class="title border-topbottom">A</div>
      <div class="item-list">
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
      </div>
    </div>
    <div class="area">
      <div class="title border-topbottom">A</div>
      <div class="item-list">
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
      </div>
    </div>
    <div class="area">
      <div class="title border-topbottom">A</div>
      <div class="item-list">
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
        <div class="item border-bottom">阿联酋</div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "CityList"
};
</script>
<style lang='stylus' scope>
@import '~styles/varibles.styl';

.border-topbottom {
  &:before {
    border-color: #cccccc;
  }

  &:after {
    border-color: #cccccc;
  }
}

.border-bottom {
  &:before {
    border-color: #cccccc;
  }
}
.list{
    overflow hidden
    position absolute
    top 1.58rem
    left 0
    right 0
    bottom 0

}

.title {
  line-height: 0.4rem;
  background: #eeeeee;
  padding-left: 0.2rem;
  color: #666;
  font-size: 0.26rem;
}

.button-list {
  padding: 0.1rem;
  overflow: hidden;
  padding: 0.1rem 0.6rem 0.1rem 0.1rem;
}

.button-wrapper {
  float: left;
  width: 33.3%;
}

.button {
  text-align: center;
  margin: 0.1rem;
  border: 0.02rem solid #ccc;
  padding: 0.1rem 0;
  boreder-radius: 0.06rem;
}

.item {
  line-height: 0.76rem;
  padding-left: 0.2rem;
}
</style>