<template>
    <div id="main-header">



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
  name: 'app',
        data() {
        return {
        }
  },
  methods: {
    },
}
</script>

<style>
  .main-header{

  }
</style>
