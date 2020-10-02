<template>
  <div id="tab-bar">
    <slot></slot>
    <!-- <div class="tab-bar-item">
      <i class="fa fa-home"></i>
      <i>首页</i>
    </div>
    <div class="tab-bar-item">
      <i class="fa fa-receipt"></i>
      <i>分类</i>
    </div>
    <div class="tab-bar-item">
      <i class="fa fa-shopping-cart"></i>
      <i>购物车</i>
    </div>
    <div class="tab-bar-item">
      <i class="fa fa-user"></i>
      <i>我的</i>
    </div> -->
  </div>
</template>

<script>
export default {};
</script>

<style>
/* @import "../../assets/css/font/css/all.css"; */
#tab-bar {
  display: flex;
  justify-content: space-around;
  background-color: #f6f6f6;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.2);
  /* line-height: 28px; */
  height: 49px;
  /* text-align: center; */
  box-sizing: border-box;
  /* padding: 10px 0; */
}


</style>