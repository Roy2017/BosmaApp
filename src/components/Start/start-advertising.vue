<template>
  <div class=" content-color content-margin">
    <div class="page-header title">最新活动</div>
    <div class="adv-content am-flexbox am-flexbox-justify-between">
      <div class="adv-items" :style="{backgroundImage: 'url('+img+')'}"></div>
      <div class="adv-items" :style="{backgroundImage: 'url('+img1+')'}"></div>
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

export default {
  name: 'slider',
  data()
     {
       return {
         img:'//www.nidosport.com/images/fdae56.png',
         img1:'//www.nidosport.com/images/cf5d86.png',
//         img2:'//www.nidosport.com/images/0a6d0e.png',
//         img3:'//www.nidosport.com/images/46969a.png',
//         img4:'//www.nidosport.com/images/1ef6ae.png',
//         img5:'//www.nidosport.com/images/0a6d0e.png',
//         img6:'//www.nidosport.com/images/46969a.png',
//         img7:'//www.nidosport.com/images/120c9b.png',
       }
     }
     ,
     methods: {
     },

     mounted(){

     }
}
</script>

<style scoped>
  .title{
    background: url('../../assets/images/pro_tb.png')no-repeat 0.24rem ;
  }
  .adv-content{
    width: 100%;
    height: auto;
    background-size: cover;
    background-repeat: no-repeat;
    padding: 0.16rem 0.12rem;
  }
  .adv-items{
    width: 49%;
    height: 27vw;
    background: black;
    background-size: cover;
    background-repeat: no-repeat;
    border-radius: 0.1rem;
    box-shadow:0.05rem 0.05rem 0.02rem #e5e5e5;
  }
</style>
