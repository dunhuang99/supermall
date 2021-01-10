<template>
  <div id="home">
    <nav-bar class="home-nav">
      <div slot="center">
        购物街
      </div>
    </nav-bar>
    <!-- <home-swiper :banners="banners"></home-swiper> -->
  </div>
</template>
<script>
    import NavBar from 'components/common/navbar/NavBar.vue'
    // import HomeSwiper from './childComps/HomeSwiper'
    import { getHomeMultidata } from 'network/home.js'

    export default {
      name: 'Home',
       data() {
        return {
          banners: [],
          recommends: []
        }
      },
      components: {
        NavBar,
        // HomeSwiper,
      },
       created() {
        getHomeMultidata().then(res => {
          this.banners = res.data.banner.list
          this.recommends = res.data.recommend.list
          console.log(this.banners);
        })
      },
    }
</script>
<style >
  .home-nav {
    background-color: var(--color-tint);
    color: #fff;
  }
</style>