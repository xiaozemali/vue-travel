<template>
  <div class="icons">
    <swiper>
      <swiper-slide v-for="(page,index) in pages" :key="index">
        <div class="icon" v-for="item in page" :key="item.id">
          <div class="icon-img">
            <div class="icon-img-content">
              <img :src="item.imgUrl" />
            </div>
          </div>
          <p class="icon-desc">{{item.desc}}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>
<script>
export default {
  name: "HomeIcons",
  data(){
      return{
          iconList:[{
              id:'0001',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'广州'
          },{
              id:'0002',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'天河区'
          },{
              id:'0003',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'海珠区'
          },{
              id:'0004',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'白云区'
          },{
              id:'0005',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'越秀区'
          },{
              id:'0006',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'荔湾区'
          },{
                id:'0007',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'黄埔区'
          },{
                id:'0008',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'花都区'
          },{
                id:'0009',
              imgUrl:'//s.qunarzz.com/homenode/images/touchheader/hotel.png',
              desc:'南沙区'
          }]
      }
  },
  computed:{
      pages(){
          const pages=[]
          this.iconList.forEach((item,index)=>{
              const page =Math.floor(index/8)
              if(!pages[page]){
                  pages[page]=[]
              }
              pages[page].push(item)
          })
          return pages
      }
  }
};
</script>
<style lang='stylus' scope>
@import '~styles/varibles.styl';
@import '~styles/mixins.styl';

.swiper-container {
  overflow: hidden;
  height: 0;
  padding-bottom: 50%;
}

.icon-desc {
  position: absolute;
  left: 0;
  right: 0;
  bottom: 0;
  height: 0.44rem;
  line-height: 0.44rem;
  color: $darkTextColor;
  text-align: center;
  ellipsis()
}

.icon {
  margin-top .1rem;
  position: relative;
  overflow: hidden;
  float: left;
  width: 25%;
  padding-bottom: 25%;
}

.icon-img {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0.44rem;
  box-sizing: border-box;
  padding-left: 0.2rem;
}

.icon-img-content {
  height: 100%;
  display: block;
  margin: 0 auto;
}

img {
  width: 80%;
}
</style>