<template>
  <div id="app">
    <tab-bar>
      <template v-slot:itemBar>
        <div class="tab-bar-item">
          <img src="./assets/img/tabbar/home.svg" alt="" />
          <div>首页</div>
        </div>
        <div class="tab-bar-item">
          <img src="./assets/img/tabbar/category.svg" alt="" />
          <div>分类</div>
        </div>
        <div class="tab-bar-item">
          <img src="./assets/img/tabbar/shopcart.svg" alt="" />
          <div>购物车</div>
        </div>
        <div class="tab-bar-item">
          <img src="./assets/img/tabbar/profile.svg" alt="" />
          <div>我的</div>
        </div>
        
      </template>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "./components/tabbar/TabBar.vue";
export default {
  name: "App",
  components: {
    TabBar,
  },
};
</script>

<style>
@import "./assets/css/base.css";
</style>
