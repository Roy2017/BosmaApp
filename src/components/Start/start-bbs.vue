<template>
  <div class=" content-color content-margin">
    <div class="page-header am-flexbox title am-flexbox-justify-between">
      Bosma社区<div class="text-sm">查看全部 &gt</div>
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
          <div class="author-tag author-tag-blue">
            有奖活动
          </div>
        </div>
        <div class="author-topic text-bold text-lg text-clamp-2 content-margin am-flexbox am-flexbox-align-top">
          <img :src="postImg1" alt=""/><img :src="postImg2" alt=""/>
          <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet asperiores debitis dolores eligendi eos fugiat, magnam,</span>
        </div>
        <div class="author-footer am-flexbox am-flexbox-justify-between">
          <div class="author-footer-looker am-flexbox am-flexbox-item">
            <img class="author-footer-icons" src="../../assets/svg/eyes.svg" alt=""/>
            <span>103</span>
          </div>
          <div class="author-footer-others am-flexbox am-flexbox-justify-between">
            <div class="am-flexbox">
              <img class="author-footer-icons" src="../../assets/svg/like.svg" alt=""/>
              <span>103</span>
            </div>
            <div class="am-flexbox">
              <img class="author-footer-icons" src="../../assets/svg/chat.svg" alt=""/>
              <span>103</span>
            </div>
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
          <div class="author-tag author-tag-blue">
            有奖活动
          </div>
        </div>
        <div class="author-topic text-bold text-lg text-clamp-2 content-margin am-flexbox am-flexbox-align-top">
          <img :src="postImg1" alt=""/><img :src="postImg2" alt=""/>
          <span>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet asperiores debitis dolores eligendi eos fugiat, magnam,</span>
        </div>
        <div class="author-footer am-flexbox am-flexbox-justify-between">
          <div class="author-footer-looker am-flexbox am-flexbox-item">
            <img class="author-footer-icons" src="../../assets/svg/eyes.svg" alt=""/>
            <span>103</span>
          </div>
          <div class="author-footer-others am-flexbox am-flexbox-justify-between">
            <div class="am-flexbox">
              <img class="author-footer-icons" src="../../assets/svg/like.svg" alt=""/>
              <span>103</span>
            </div>
            <div class="am-flexbox">
              <img class="author-footer-icons" src="../../assets/svg/chat.svg" alt=""/>
              <span>103</span>
            </div>
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
         postImg1:'//www.nidosport.com/images/e44051.png',
         postImg2:'//www.nidosport.com/images/3b3932.png',
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
  /*主题 一行*/
  .author-topic{
    width: 100%;
    line-height: 1.5;

  }
  .author-topic img{
    display: inline-block;
    width: .44rem;
    height: .44rem;
    vertical-align: middle;
    margin-right: 0.08rem;
  }
  /*底栏*/
  .author-footer{
    width: 100%;
    margin-top: .32rem

  }
  .author-footer-looker{
    /*height: auto;*/
    /*margin-right: 2%;*/
    /*background: black;*/
  }
  .author-footer-others>div:nth-child(n+2){
    margin-left: 0.16rem;
  }
  .author-footer-icons{
    width: 0.36rem;
    height: 0.36rem;
    margin-right: 0.08rem;

  }
  /*查看更多*/
  .choose-getMore{
    padding: 0.32rem;
    text-align: center;
    border-top: 1px solid #e5e5e5;
  }
  /*渐变标签*/
  .author-tag{
    display: inline-block;
    padding: .02rem .12rem;
    vertical-align: top;
    font-size: .2rem;
    letter-spacing: .04rem;
    color: #fff;
    border-radius: .08rem;
    -webkit-flex: none;
  }
  .author-tag-yellow {
    background-image: linear-gradient(90deg,#ffab3e,#ffcc8b);
  }
  .author-tag-purple {
    background-image: linear-gradient(90deg,#d06bdc,#e4a9eb);
  }
  .author-tag-blue {
    background-image: linear-gradient(90deg,#216ff0,#699df5);
  }
</style>
