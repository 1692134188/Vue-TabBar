

<template>
  <tab-bar>
    <template v-slot:itemBar>
      <tab-bar-item path="/home" activeColor="blue">
        <template v-slot:activeImgSlot>
          <img src="../../assets/img/tabbar/home_active.svg" alt="" />
        </template>
        <template v-slot:imgSlot>
          <img src="../../assets/img/tabbar/home.svg" alt="" />
        </template>
        <template v-slot:textSlot> 首页</template>
      </tab-bar-item>
      <tab-bar-item path="/category">
        <template v-slot:activeImgSlot>
          <img src="~assets/img/tabbar/category_active.svg" alt="" />
        </template>
        <template v-slot:imgSlot>
          <img src="~assets/img/tabbar/category.svg" alt="" />
        </template>
        <template v-slot:textSlot> 分类</template>
      </tab-bar-item>
      <tab-bar-item path="/cart">
        <template v-slot:activeImgSlot>
          <img src="~assets/img/tabbar/shopcart_active.svg" alt="" />
        </template>
        <template v-slot:imgSlot>
          <img src="~assets/img/tabbar/shopcart.svg" alt="" />
        </template>
        <template v-slot:textSlot> 购物车</template>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <template v-slot:activeImgSlot>
          <img src="~assets/img/tabbar/profile_active.svg" alt="" />
        </template>
        <template v-slot:imgSlot>
          <img src="~assets/img/tabbar/profile.svg" alt="" />
        </template>
        <template v-slot:textSlot> 我的</template>
      </tab-bar-item>
    </template>
  </tab-bar>
</template>

<script>
import TabBar from "components/tabbar/TabBar.vue";
import TabBarItem from "components/tabbar/TabBarItem.vue";

export default {
  name: "MainTabBar",
  components: {
    TabBar,
    TabBarItem,
  },
};
</script>