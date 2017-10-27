<template>
  <div class="am-flexbox items content-color">
    <a href="" class="am-flexbox " >
      <div class="items-logo" :style="{backgroundImage: 'url('+img+')'}"></div>
      <p>每日签到</p>
    </a>
    <a href="" class="am-flexbox" >
      <div class="items-logo" :style="{backgroundImage: 'url('+img1+')'}"></div>
      <p>每日签到</p>
    </a>
    <a href="" class="am-flexbox" >
      <div class="items-logo" :style="{backgroundImage: 'url('+img2+')'}"></div>
      <p>每日签到</p>
    </a>
    <a href="" class="am-flexbox" >
      <div class="items-logo" :style="{backgroundImage: 'url('+img3+')'}"></div>
      <p>每日签到</p>
    </a>
    <a href="" class="am-flexbox" >
      <div class="items-logo" :style="{backgroundImage: 'url('+img4+')'}"></div>
      <p>每日签到</p>
    </a>
    <a href="" class="am-flexbox" >
      <div class="items-logo" :style="{backgroundImage: 'url('+img5+')'}"></div>
      <p>每日签到</p>
    </a>
    <a href="" class="am-flexbox" >
      <div class="items-logo" :style="{backgroundImage: 'url('+img6+')'}"></div>
      <p>中秋礼遇</p>
    </a>
    <a href="" class="am-flexbox" >
      <div class="items-logo" :style="{backgroundImage: 'url('+img7+')'}"></div>
      <p>更多</p>
    </a>



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
         img:'//www.nidosport.com/images/3bba86.png',
         img1:'//www.nidosport.com/images/1d2f3e.png',
         img2:'//www.nidosport.com/images/0a6d0e.png',
         img3:'//www.nidosport.com/images/46969a.png',
         img4:'//www.nidosport.com/images/1ef6ae.png',
         img5:'//www.nidosport.com/images/0a6d0e.png',
         img6:'//www.nidosport.com/images/46969a.png',
         img7:'//www.nidosport.com/images/120c9b.png',
       }
     }
     ,
     methods: {
     },

     mounted(){

     }
}
</script>

<style>
  .items{
    width: 100%;
    height: 3.4rem;
    padding: 0.24rem;
    flex-wrap: wrap;
  }
  .items a{
    width: 20%;
    height: auto;
    /*padding-bottom: 20%;*/
    /*background-position: ;*/
    background: transparent;
    flex-direction: column;

  }
  .items a:nth-child(n+6){
    margin-top: 0.16rem;
  }
  .items-logo{
    width: 0.9rem;
    height: 0.9rem;
    background-size: cover;
    background-repeat: no-repeat;
  }
  .items-logo+p{
    margin-top: 0.16rem;
    font-size: .24rem!important;
  }
</style>
