<!--  -->
<template>
   <tab-bar>
    <tab-bar-item path="/home">
      <img slot="item-icon" src="~assets/img/tabbar/icon01.png" alt="">
      <img slot="item-icon-active" src="~assets/img/tabbar/icon01_active.png" alt="">
      <div slot="item-text">
        首页
      </div>
    </tab-bar-item>
    <tab-bar-item path="/category">
      <img slot="item-icon" src="~assets/img/tabbar/icon02.png" alt="">
      <img slot="item-icon-active" src="~assets/img/tabbar/icon02_active.png" alt="">
      <div slot="item-text">
        分类
      </div>
    </tab-bar-item>
    <tab-bar-item path="/cart">
      <img slot="item-icon" src="~assets/img/tabbar/icon03.png" alt="">
      <img slot="item-icon-active" src="~assets/img/tabbar/icon03_active.png" alt="">
      <div slot="item-text">
        购物车
      </div>
    </tab-bar-item>
    <tab-bar-item path="/profile">
      <img slot="item-icon" src="~assets/img/tabbar/icon04.png" alt="">
      <img slot="item-icon-active" src="~assets/img/tabbar/icon04_active.png" alt="">
      <div slot="item-text">
        我的
      </div>
    </tab-bar-item>
   </tab-bar>
</template>

    <script>
    import TabBarItem from 'components/common/tabbar/TabBarItem'
    import TabBar from 'components/common/tabbar/TabBar'

    export default {
        components: { 
            TabBarItem,
            TabBar 
        },
    }
</script>
<style >

</style>