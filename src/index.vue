<template>
  <div class="app-wrapper">
    <home-header></home-header>
    <!-- <top-channel></top-channel> -->
    <tab-bar></tab-bar>
  </div>
</template>

<style>
  /* 全局 */
  body {
    margin: 0;
    padding: 0;
    background-color: #f4f44f;
    color: #333333;
  }
</style>
// 作用于局部
<style scoped>
  .app-wrapper {
    background-color: #f4f4f4;
  }
  .r-box {
    position: absolute;
    top: 0;
    right: 0;
    right: 0;
    bottom: 0;
  }
</style>

<script>
  import util from './assets/util';
  import tabBar from './assets/components/tabBar.vue';
  import Header from './assets/components/Header.vue';
  export default {
    // 组件
    "components":{
      'home-header':Header,
      'tab-bar':tabBar
    },
    data: {

    },
    // 生命周期，组件创建
    created() {
      util.initIconFont();
    },
    methods: {
  
    }
  }
</script>