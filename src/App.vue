<template>
  <div id="main">
    <v-header></v-header>
    <div id="tab">
      <router-link class="tab-item" to="/goods">商品</router-link>
      <router-link class="tab-item" to="/ratings">评论</router-link>
      <router-link class="tab-item" to="/seller">商家</router-link>
    </div>
    <div id="content">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import header from './components/header/header.vue'
export default{
  components: {
    'v-header':header
  }
}
</script>

<style lang="less" scoped>
  #tab{
    display: flex;
    .tab-item{
      height: 40px;
      line-height: 40px;
      text-align: center;
      flex: 1;
    }
  }
</style>
