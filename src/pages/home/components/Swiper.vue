<template>
<div class="wrapper">
  <swiper :options="swiperOptions">
    <swiper-slide v-for="item in swiperList" :key="item.id">
        <img class="swpier-img"  :src="item.imgUrl"> 
    </swiper-slide>

    </swiper-slide>
    <div class="swiper-pagination" slot="pagination">
    </div>
  </swiper>
  </div>
</template>
<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOptions: {
          pagination:'.swiper-pagination',
          loop:true
      },
      swiperList:[{
        id:'0001',
        imgUrl:'https://imgs.qunarzz.com/vc/e3/a1/71/f498dfd3bed948d623c9093252.jpg_92.jpg'
      },{
        id:'0002',
        imgUrl:'https://imgs.qunarzz.com/vc/6d/9f/35/b8ad5468f73fd60ec0ced086f6.jpg_92.jpg'
      }]
    }
  }
};
</script>

<style lang="stylus" scoped>

.wrapper{
    overflow:hidden;
    width:100%;
    height 0;
    padding-bottom:31.25%;
    background :#eee;
}
    
.swpier-img{
    width: 100%
}

</style> 
