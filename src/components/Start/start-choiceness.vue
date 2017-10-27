<template>
  <div class=" content-color content-margin">
    <div class="page-header am-flexbox title am-flexbox-justify-between">
      Bosma精选<div class="text-sm">查看全部 &gt</div>
    </div>

    <div class="choose-content am-flexbox am-flexbox-dir-column">
      <div class="choose-items am-flexbox am-flexbox-dir-column" >
        <div class="author am-flexbox am-flexbox-item am-flexbox-justify-between am-flexbox-align-top">
          <div class="author-avatar bg-cover" :style="{backgroundImage: 'url('+authorImg+')'}">
            <img class="author-avatar-svip" src="//www.nidosport.com/images/6abded.png">
          </div>
          <div class="author-avatar-content am-flexbox-item am-flexbox am-flexbox-dir-column am-flexbox-align-top">
            <div class="author-name am-flexbox">
              <span class="author-name-vip text-md text-bold">我的名字</span>
              <div class="author-name-badge bg-cover" :style="{backgroundImage: 'url('+badgeImg1+')'}">
              </div>
              <div class="author-name-badge bg-cover" :style="{backgroundImage: 'url('+badgeImg1+')'}">
              </div>
            </div>
            <div class="author-date">1天6时前</div>
          </div>
        </div>
        <div class="author-text text-md text-clamp-2 content-margin">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet asperiores debitis dolores eligendi eos fugiat, magnam, maxime neque officia quas quibusdam reprehenderit, totam vitae. Excepturi molestias, odit. Ad, sit, temporibus.</div>
        <div class="author-pic-content content-margin am-flexbox">
          <div class="author-pic-items am-flexbox">
            <img src="../../assets/upLoad/20161205034256661.jpg" alt=""/>
          </div><div class="author-pic-items am-flexbox">
          <img src="../../assets/upLoad/20161205034430033.jpg" alt=""/>
        </div><div class="author-pic-items am-flexbox">
          <img src="../../assets/upLoad/20161205034741177.jpg" alt=""/>
        </div>
        </div>
      </div>

    </div>
    <div class="choose-content am-flexbox am-flexbox-dir-column">
      <div class="choose-items am-flexbox am-flexbox-dir-column" >
        <div class="author am-flexbox am-flexbox-item am-flexbox-justify-between am-flexbox-align-top">
          <div class="author-avatar bg-cover" :style="{backgroundImage: 'url('+authorImg+')'}">
            <img class="author-avatar-svip" src="//www.nidosport.com/images/6abded.png">
          </div>
          <div class="author-avatar-content am-flexbox-item am-flexbox am-flexbox-dir-column am-flexbox-align-top">
            <div class="author-name am-flexbox">
              <span class="author-name-vip text-md text-bold">我的名字</span>
              <div class="author-name-badge bg-cover" :style="{backgroundImage: 'url('+badgeImg1+')'}">
              </div>
              <div class="author-name-badge bg-cover" :style="{backgroundImage: 'url('+badgeImg1+')'}">
              </div>
            </div>
            <div class="author-date">1天6时前</div>
          </div>
        </div>
        <div class="author-text text-md text-clamp-2 content-margin">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet asperiores debitis dolores eligendi eos fugiat, magnam, maxime neque officia quas quibusdam reprehenderit, totam vitae. Excepturi molestias, odit. Ad, sit, temporibus.</div>
        <div class="author-pic-content content-margin am-flexbox">
          <div class="author-pic-items am-flexbox">
            <img src="../../assets/upLoad/20161205034256661.jpg" alt=""/>
          </div><div class="author-pic-items am-flexbox">
          <img src="../../assets/upLoad/20161205034430033.jpg" alt=""/>
        </div><div class="author-pic-items am-flexbox">
          <img src="../../assets/upLoad/20161205034741177.jpg" alt=""/>
        </div>
        </div>
      </div>

    </div>

    <div class="choose-getMore text-md text-desc">
      ->查看更多
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
         authorImg:'https://api.nidosport.com/file/getimg/123562/thumb',
         badgeImg1:'//www.nidosport.com/common/images/level/vip2.png',
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

<style>
  .title{
    background: url('../../assets/images/pro_tb.png')no-repeat 0.24rem ;
  }
  .choose-content{
    width: 100%;
    height: auto;
    border-top: 1px solid #e5e5e5;
    padding: 0 0.24rem;
    flex-direction: column;
  }
  .choose-items{
    padding: 0.36rem 0;
    width: 100%;
    height: auto;
    /*background: black;*/
  }
  /*头像*/
  .author{
    width: 100%;
  }
  .author-avatar{
    width: 0.8rem;
    height: 0.8rem;
    border-radius: 50%;
    position: relative;
  }
  .author-avatar-svip{
    position: absolute; bottom: 0px; right: -5px;
    width: .3rem;
    height: .3rem;
  }
  .author-avatar-content{
    height: 100%;
    margin-left: 0.16rem;
    align-items: flex-start;
  }
  .author-name{
    height: 60%;
  }
  .author-name-badge{
    width: .4rem;
    height: .4rem;
    margin: 0 0.05rem;
    display: inline-block;

  }
  .author-name-vip{
    color: red !important;
  }
  .author-date{
    height: 40%;
  }
  /*文字 两行*/
  .author-text{
    width: 100%;
    line-height: 1.5;
  }
  /*图片*/
  .author-pic-content{
    width: 100%;

  }
  .author-pic-items{
    width: 33%;
    height: auto;
    margin-right: 2%;
    /*background: black;*/
  }
  .author-pic-items img{
    width: 100%;
    /*display: none;*/
  }
  /*查看更多*/
  .choose-getMore{
    padding: 0.32rem;
    text-align: center;
    border-top: 1px solid #e5e5e5;
  }
</style>
