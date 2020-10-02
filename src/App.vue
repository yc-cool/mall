<template>
  <div id="app">
    <router-view></router-view>
    <tab-bar>
      <tab-bar-item path="/home" activeColor='blue'>
        <i class="fa fa-home"></i>
        <span>首页</span>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <i class="fa fa-receipt"></i>
        <i>分类</i>
      </tab-bar-item>
      <tab-bar-item path="/cart">
        <i class="fa fa-shopping-cart"></i>
        <i>购物车</i>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <i class="fa fa-user"></i>
        <i>我的</i>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "./components/common/tabbar/TabBar"
import TabBarItem from "./components/common/tabbar/TabBarItem"
export default {
  name: 'App',
  components: {
    TabBarItem,
    TabBar
  }
}
</script>

<style>
@import "./assets/css/reset.css";
/* @import "./assets/css/normalize.css" */
/* @import url('./assets/css/base.css'); */
@import "./assets/css/base.css";

</style>
