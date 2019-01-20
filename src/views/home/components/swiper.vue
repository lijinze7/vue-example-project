<template>
  <div class="swiper">
    <swiper :options="swiperOption" ref="mySwiper">
      <!-- slides -->
      <swiper-slide class="slide" v-for="item in slideList">
        <img :src="item.imgUrl" />
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
  
</template>

<script>
  export default {
    name: 'HomeSwiper',
    data() {
      return {
        swiperOption: {
          // some swiper options/callbacks
          // 所有的参数同 swiper 官方 api 参数
          // ...
          pagination: '.swiper-pagination',
          loop: true
        },
        slideList: [
          {
            id: "001",
            imgUrl: require("../../../../static/img/slide1.jpg")
          },
          {
            id: "002",
            imgUrl: require("../../../../static/img/slide2.jpg")
          },
          {
            id: "003",
            imgUrl: require("../../../../static/img/slide3.jpg")
          }
        ]
      }
    }
  }
</script>

<style scoped>
.swiper{
    overflow: hidden;
    width: 100%;
    height: 0;
    padding-bottom: 26.66%;
}

.swiper .slide img{
    width: 100%;
}

</style>