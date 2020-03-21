<template>
  <div class="home">
    <NavBar class="nav-bar">
      <div class="center" slot="center">
        <img src="https://www.rakuten.ne.jp/gold/fedonline/images/huang.png">
      </div>
    </NavBar>
    <carousel class="carousel"></carousel>
    <banner/>
    <Main></Main>
  </div>
</template>

<script>
import NavBar from '@/components/navbar/NavBar.vue'
import carousel from './children/carousel'
import Main from './children/main'
import banner from './children/banner'
export default {
  name: 'home',
  data () {
    return {
    }
  },
  components: {
    NavBar,
    carousel,
    Main,
    banner
  }
}
</script>
<style scoped>
  .home {
    height: 999999px;
    position: relative;
  }
  .nav-bar {
    width: 100%;
    background-color: #000;
    position: fixed;
    top: 0;
    z-index: 9999;
  }
  .nav-bar .center img {
    width: 70px;
    margin-top: 5px;
  }
  .nav-bar .left {
    width: 60px;
  }
  .carousel {
    margin-top: 44px;
  }
</style>
