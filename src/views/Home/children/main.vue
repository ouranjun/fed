<template>
  <tabs v-model="active" sticky animated>
      <tab title="メンズファッション">
          <div class="man" v-for="(item, index) in manImg" :key="index" >
              <a :href="item.linkUrl">
              <img :src="item.picUrl" alt="">
              </a>
          </div>
      </tab>
      <tab title="ペット用品">内容 2</tab>
      <tab title="美容·健康">内容 3</tab>
      <tab title="レディースファッション">内容 4</tab>
  </tabs>
</template>

<script>
import {Tab, Tabs} from 'vant'
import 'vant/lib/tab/style'
import 'vant/lib/tabs/style'
export default {
  name: 'Main',
  data () {
    return {
      active: 0,
      manImg: [
        {
          linkUrl: 'https://item.rakuten.co.jp/fedonline/hl701/',
          picUrl: require('@/assets/main/701-1-5.jpg')
        },
        {
          linkUrl: 'https://item.rakuten.co.jp/fedonline/hl-901/',
          picUrl: require('@/assets/main/901-20.jpg')
        },
        {
          linkUrl: '#',
          picUrl: require('@/assets/main/2.jpg')
        },
        {
          linkUrl: 'https://item.rakuten.co.jp/fedonline/lh706/',
          picUrl: require('@/assets/main/no3.jpg')
        },
        {
          linkUrl: 'https://item.rakuten.co.jp/fedonline/22027-black/',
          picUrl: require('@/assets/main/no4.jpg')
        },
        {
          linkUrl: '#',
          picUrl: require('@/assets/main/no3+no4.jpg')
        },
        {
          linkUrl: 'https://item.rakuten.co.jp/fedonline/lh-729/',
          picUrl: require('@/assets/main/NO5.jpg')
        },
        {
          linkUrl: 'https://item.rakuten.co.jp/fedonline/ts99009/',
          picUrl: require('@/assets/main/no6.jpg')
        },
        {
          linkUrl: 'https://item.rakuten.co.jp/fedonline/1908/',
          picUrl: require('@/assets/main/1908.jpg')
        }
      ]
    }
  },
  components: {
    Tab,
    Tabs
  }
}
</script>

<style scoped>
    .man img{
        width: 100%;
    }
</style>>
