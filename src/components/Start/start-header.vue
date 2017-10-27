<template>
  <div class="main-header content-color am-flexbox  am-flexbox-justify-between">
    <div class="am-flexbox  main-header-lside">&lt 返回</div>
    <div class="am-flexbox am-flexbox-item am-flexbox-justify-center">
      <img src="../../assets/images/logo.png" alt="" class="main-header-logo"/></div>
    <div class="am-flexbox  main-header-rside am-flexbox-justify-end"><img
      src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACsAAAA7CAMAAADVVYNpAAAAt1BMVEUAAAAAAAAAAAAAAAAJCQkAAAAAAAAAAAAAAAAzMzMzMzMAAAAAAAAAAAAzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMAAAAzMzMzMzMzMzMzMzMzMzMzMzMAAAAzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMzMAAAAzMzMzMzMzMzMAAABxsDV9AAAAO3RSTlMAzIhVEZl33e4N8qpmRL9eMCCnhIBnPhr2ycSwdEIIA+vl3Lu5s5aObU0i+uDYzp5VNyjv03tTSDMkVqNI6xAAAAKXSURBVEjHjJPHbsMwEET34It5kGV1ucgFrnBvMZL3//+VEFS1CvJOBDkkZ8kd+cAeeKuTUmq52vq2dBE4lLHercrZBc0jXjvj0QONEzZLf5aAtd33RdMPXAtQgyapC5y+qpZiYFuX7oBLbXbTNPsCfKmzj8CTCjdgKk1MaysxTKQZH9SHWUva2IIjOQnQl1aOUDzzBFxpxyuVPZszn5nhsCIaJuZbIo6Scs8NrSl/0yArwoH0kG8rsxDCWApGWRVXOAdmN/A2d1Y/aUxktL0DcP0zgyY02pZz5QTQEx/ISktOvCrdtExLtgA2ejN5mcmtGpJe7gZQsjDabtYAB5kDqKRTai6P5IymO4azh/Hgohl0au9oVvqdSkEJyq363hf9Atjp4CkGhyJxAQsxLMlSs4sKEz2Fm/e0uhehOaRBCneed81aa0W0mfiTDcRh8bpe2BywJ5o4N2PDXNro21O7FJMF7OVfJL/dk0FPxSAMgCm0hSdM48WDN91tB6NGk/eS/v/fZaEusF3k7JdssOyjlKY8106Y4157d8681E64TYifD9+a6+vHhPpk9bi4Cd6sCabQSzZbLWvw25z7+HX38u7+B55cBxUblNFaQsVLaeNS14kCDkRs0oEInQjVhRBY3RyUfHC97gY1XtN+X0Fdb7+PLkIMDfzDrVETNCRY8PrZ3MWTlMPhABKhjomcudH73NzNe3YjMeO2Riax3XoOea9MB/UpUSRfT24Uq0wHA68p5cAgkDksQw6gCWTqqhcBsvyvnEFoOBuvmmHp7haQYYccjjXDVDi5jp3bWC03or2+nKI/uXCcgN9dF+V6dtEwFyXsLkmMy9GVneaWpL1H6tKaCpLw6DKhwdTistsAiiOmrS61QvwAco5fg+S7TigAAAAASUVORK5CYII="
      alt="" style="width: 0.43rem; height: 0.59rem;"/></div>

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
    height: 0.96rem;
    width: 100%;
  }
  .main-header-lside{
    width: 2.4rem;
    padding-left: .24rem;
  }
  .main-header-rside{
    width: 2.4rem;
    padding-right: .24rem;
  }
  .main-header-logo{
    position: relative;
    top:0.2rem;
  }
</style>
