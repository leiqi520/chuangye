<script setup>
  import { ref } from 'vue'
  const active = ref(0)
  const active_bottom = ref(0)
</script>

<template>
  <van-nav-bar title="创业平台" />
  <van-swipe class="my-swipe" :autoplay="3000" indicator-color="white">
    <van-swipe-item>
      <img src="../assets/banner1.png" alt="" />
    </van-swipe-item>
    <van-swipe-item>
      <img src="../assets/banner2.png" alt="" />
    </van-swipe-item>
    <van-swipe-item>
      <img src="../assets/banner3.png" alt="" />
    </van-swipe-item>
  </van-swipe>
  <van-row id="navs">
    <van-col span="6">
      <img src="../assets/nav1.png" alt="" />
      <p>创业时讯</p>
    </van-col>
    <van-col span="6">
      <img src="../assets/nav2.png" alt="" />
      <p>创业时讯</p>
    </van-col>
    <van-col span="6">
      <img src="../assets/nav3.png" alt="" />
      <p>创业时讯</p>
    </van-col>
    <van-col span="6">
      <img src="../assets/nav4.png" alt="" />
      <p>创业时讯</p>
    </van-col>
  </van-row>
  <van-tabs v-model:active="active">
    <van-tab title="创业时讯">
      <van-row>
        <van-col span="16">
          <h4>标题</h4>
          <p>2022年</p>
        </van-col>
        <van-col span="8">
          <img src="../assets/imgs/bingge.jpg" alt="" />
        </van-col>
      </van-row>
    </van-tab>
    <van-tab title="标签 2">内容 2</van-tab>
    <van-tab title="标签 3">内容 3</van-tab>
    <van-tab title="标签 4">内容 4</van-tab>
  </van-tabs>
  <van-tabbar v-model="active_bottom">
    <van-tabbar-item icon="home-o">标签</van-tabbar-item>
    <van-tabbar-item icon="search">标签</van-tabbar-item>
    <van-tabbar-item icon="friends-o">标签</van-tabbar-item>
    <van-tabbar-item icon="setting-o">标签</van-tabbar-item>
  </van-tabbar>
</template>

<style scoped>
.van-swipe-item img {
  width: 100%;
}
#navs {
  padding: 10px;
  text-align: center;
}
#navs img {
  width: 55px;
}
</style>
