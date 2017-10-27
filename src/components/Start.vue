<template>
  <div class="start">
    <MainHeader></MainHeader>
    <MainSlider></MainSlider>
    <MainItems></MainItems>
    <MainAdv></MainAdv>
    <MainChoiceness></MainChoiceness>
    <Mainbbs></Mainbbs>
    <MainNewUser></MainNewUser>
    <MainVideo></MainVideo>
  </div>
</template>

<script>
import MainHeader from '@/components/Start/start-header'
import MainSlider from '@/components/Start/start-slider'
import MainItems from '@/components/Start/start-items'
import MainAdv from '@/components/Start/start-advertising'
import MainChoiceness from '@/components/Start/start-choiceness'
import Mainbbs from '@/components/Start/start-bbs'
import MainNewUser from '@/components/Start/start-newuser'
import MainVideo from '@/components/Start/start-video'

export default {
  name: 'start',
  methods:{
    jump(path){
      this.$parent.jump(path);
    }
  },
  components:{
    MainHeader,
    MainSlider,
    MainItems,
    MainAdv,
    MainChoiceness,
    Mainbbs,
    MainNewUser,
    MainVideo,

  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
