<template>
  <div class=" content-color content-margin">
    <div class="page-header am-flexbox title am-flexbox-justify-between">
      视频专区<div class="text-sm">查看全部 &gt</div>
    </div>

    <div class="video-choose-content am-flexbox am-flexbox-dir-column">
      <div class="video-choose-items am-flexbox am-flexbox-align-stretch" >
        <div class="video-pic">
          <img :src="videoImg1" alt=""/>
          <img src="../../assets/images/video_logo.png" class="video-playlogo" alt=""/>
        </div>
        <div class="video-content am-flexbox am-flexbox-item am-flexbox-dir-column am-flexbox-justify-between am-flexbox-align-top">
          <div>
            <div class="video-item text-lg text-clamp-2">
              <span>广州大道钓鱼看望远镜广州大道钓鱼看望远镜州大道钓鱼看望远镜广州大道钓鱼看望远镜</span>
            </div>
            <div class="author-tag author-tag-blue">新人</div>
          </div>
          <div class="video-footer am-flexbox am-flexbox-justify-between">
            <span class="am-flexbox-item">1天0时前</span>
            <div class="am-flexbox">
              <img src="../../assets/svg/eyes.svg" alt="" class="video-footer-icon"/>
              <span>109</span>
            </div>

          </div>
        </div>
      </div>

    </div>
    <div class="video-choose-content am-flexbox am-flexbox-dir-column">
      <div class="video-choose-items am-flexbox am-flexbox-align-stretch" >
        <div class="video-pic">
          <img :src="videoImg2" alt=""/>
          <img src="../../assets/images/video_logo.png" class="video-playlogo" alt=""/>
        </div>
        <div class="video-content am-flexbox am-flexbox-item am-flexbox-dir-column am-flexbox-justify-between am-flexbox-align-top">
          <div>
            <div class="video-item text-lg text-clamp-2">
              <span>广州大道钓鱼看望远镜</span>
            </div>
            <div class="author-tag author-tag-blue">新人</div>
          </div>
          <div class="video-footer am-flexbox am-flexbox-justify-between">
            <span class="am-flexbox-item">1天0时前</span>
            <div class="am-flexbox">
              <img src="../../assets/svg/eyes.svg" alt="" class="video-footer-icon"/>
              <span>109</span>
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
         videoImg1:'http://oqe980qdu.bkt.clouddn.com/J2S-j4Nt-P9x22vhOjGRRItgaYg=/ltgPpV9VG8ncWy60I4cwqoYAXwDd/image_proportion_cut',
         videoImg2:'http://oqe980qdu.bkt.clouddn.com/J2S-j4Nt-P9x22vhOjGRRItgaYg=/lomX-UwpQR-phrWNorH3e0weRJTo/image_proportion_cut',
//         postImg1:'//www.nidosport.com/images/e44051.png',
//         postImg2:'//www.nidosport.com/images/3b3932.png',
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
  .video-choose-content{
    width: 100%;
    height: auto;
    /*border-top: 1px solid #e5e5e5;*/
    padding: 0 0.24rem;
    flex-direction: column;
  }
  .video-choose-items{
    padding-top: 0.36rem;
    width: 100%;
    height: auto;

  }
  /*视频图*/
  .video-pic{
    width: 2.76rem;
    height: 1.8rem;

    position: relative;
    -webkit-flex: none;
  }
  .video-pic>img:first-child{
    width: 100%;
    height: 100%;
    border-radius: 0.08rem;

  }
  .video-playlogo{
    width: 0.8rem;
    height: 0.8rem;
    position: absolute;
    left: 50%;
    top: 50%;
    opacity: 0.8;
    -webkit-transform: translate(-50%,-50%);
    transform: translate(-50%,-50%);
  }
  .video-content{
    margin-left: .16rem;
  }
  .video-item{

  }
  /*底栏*/
  .video-footer{
    width: 100%;
  }
  .video-footer-icon{
    width: 0.36rem;
    height: 0.36rem;
    margin-right: 0.08rem;
    opacity: 0.6;
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
    margin-top: 0.08rem;
    -webkit-transform : scale(0.84,0.84) ;
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
