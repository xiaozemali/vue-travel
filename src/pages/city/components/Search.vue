<template>
<div class="search">
<input class="search-input" type="text" placeholder="输入城市名或拼音"/>
</div>
</template>
<script>
export default {
    name:'CitySearch'
}
</script>
<style lang='stylus' scope>
@import '~styles/varibles.styl';
.search
    background $bgColor
    height .72rem
    padding 0 .1rem
    .search-input
        box-sizing border-box
        padding 0 .1rem
        width  100%
        height .62rem
        line-height .62rem
        text-align center
        border-radius .08rem
        color #666
</style>