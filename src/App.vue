<template>
  <div id="app">
    <tab-bar>
      <template v-slot:itemBar>
        <tab-bar-item>
          <template v-slot:imgSlot>
            <img src="./assets/img/tabbar/home.svg" alt="" />
          </template>
          <template v-slot:textSlot> 首页</template>
        </tab-bar-item>
        <tab-bar-item>
          <template v-slot:imgSlot>
            <img src="./assets/img/tabbar/category.svg" alt="" />
          </template>
          <template v-slot:textSlot> 分类</template>
        </tab-bar-item>
        <tab-bar-item>
          <template v-slot:imgSlot>
            <img src="./assets/img/tabbar/shopcart.svg" alt="" />
          </template>
          <template v-slot:textSlot> 购物车</template>
        </tab-bar-item>
        <tab-bar-item>
          <template v-slot:imgSlot>
            <img src="./assets/img/tabbar/profile.svg" alt="" />
          </template>
          <template v-slot:textSlot> 我的</template>
        </tab-bar-item>
      </template>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "./components/tabbar/TabBar.vue";
import TabBarItem from "./components/tabbar/TabBarItem.vue";
export default {
  name: "App",
  components: {
    TabBar,
    TabBarItem,
  },
};
</script>

<style>
@import "./assets/css/base.css";
</style>
