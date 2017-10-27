<template>
  <div class="am-flexbox">
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide">
          <a href="">
            <img src="../../../static/img/20170516032557579.jpg" alt=""/>
          </a>
        </div>
        <div class="swiper-slide">
          <a href="">
            <img src="../../../static/img/20170719040458693.jpg" alt=""/>
          </a>
        </div>
        <div class="swiper-slide">
          <a href="" :style="{backgroundImage: 'url(' + img + ')'}"></a>
        </div>

      </div>
      <!-- Add Pagination -->
      <div class="swiper-pagination"></div>
    </div>


  </div>
</template>


<script>
     /*
打通父子之间所有数据和方法的共享：
　　　　　　父模板：<child ref="子名称"></child>
　　　　　　父访问子:	父组件: this..子名称.子数据/方法名()
　　　　　　子访问父:	子组件: this..子数据/方法名()
 */
import Swiper from '../../../static/js/swiper.min.js'
export default {
  name: 'slider',
  data()
     {
       return {
         img:'https://api.nidosport.com/static/uploads/jpg/20171007/59d88d787f567.jpg'
       }
     }
     ,
     methods: {
     },

     mounted(){


       this.$nextTick(function () {
         /* 焦点图 */
         var mySwiper = new Swiper('.swiper-container', {
           loop: true,

           // 如果需要分页器
           pagination: {
             el: '.swiper-pagination',
             clickable:true,
             type:'bullets',
           },



           // 如果需要前进后退按钮
           /* nextButton: '.swiper-button-next',
     prevButton: '.swiper-button-prev',   */
//           grabCursor: true,

//           spaceBetween: 30,
//           centeredSlides: true,
//           autoplay: 2000
  });
})
}
}
</script>

<style>
  .swiper-container {
    width: 100%;
    height: 40vw;
  }
  .swiper-slide {
    text-align: center;

    /* Center slide text vertically */
    display: -webkit-box;
    display: -ms-flexbox;
    display: -webkit-flex;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    -webkit-justify-content: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    -webkit-align-items: center;
    align-items: center;
  }
  .swiper-slide a{
    width: 100%;
    height: 100%;
    background-repeat: no-repeat;
    background-size: cover;



  }
  .swiper-pagination-bullet {
    border-radius: 1px !important;
    width: 0.2rem !important;
    height: 0.08rem !important;

  }
  .swiper-pagination-bullet-active{
    background: #999 !important;
  }
  .swiper-slide img{
    width: 100%;
    height: 100%;
  }
</style>
