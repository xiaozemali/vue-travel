<template>
  <div>
    <ul class="list">
      <li class="item" v-for="(item,key) in cities" :key="key">{{key}}</li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "CityAlphabet",
  props:{
      cities:Object
  }
};
</script>
<style lang='stylus' scoped>
@import '~styles/varibles.styl';

.list {
  position: absolute;
  top: 6.5rem;
  right: 0;
  bottom: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 0.6rem;
  color: $bgColor;
  padding-left 6.9rem;
}

.item {
    line-height .4rem
    text-align center
}
</style>