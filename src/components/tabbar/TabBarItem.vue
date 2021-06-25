<template>
  <div class="tab-bar-item" @click="itemClick">
    <div v-show="isActive"><slot name="activeImgSlot"></slot></div>
    <div v-show="!isActive"><slot name="imgSlot"></slot></div>
    <div><slot name="textSlot"></slot></div>
  </div>
</template>

<script>
export default {
  name: "TabBarItem",
  props:{path: String},
  computed: {
    isActive() {
      return this.$route.path.indexOf(this.path) != -1
    },
  },
  methods:{
    itemClick(){
      this.$router.push(this.path)
    }
  }
};
</script>

<style scoped>
.tab-bar-item {
  flex: 1;
  text-align: center;
  height: 49px;
  font-size: 14px;
}

.tab-bar-item img {
  width: 24px;
  height: 24px;
  margin-top: 3px;
  vertical-align: middle;
  margin-bottom: 2px;
}
</style>