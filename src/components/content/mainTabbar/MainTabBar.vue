<template>
    <div>
    <tab-bar>
      <tabbar-item path='/home' activeColor = 'deeppink'>
        <template v-slot:item-icon>
          <img src="~assets/img/tabbar/home.svg">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/home_active.svg">
        </template>
        <template v-slot:item-text>
          <div>首页</div>
        </template>   
      </tabbar-item>
      <tabbar-item path="category" activeColor = 'deeppink'>
        <template v-slot:item-icon>
          <img src="~assets/img/tabbar/category.svg">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/category_active.svg">
        </template>
        <template v-slot:item-text>
          <div>分类</div>
        </template> 
      </tabbar-item>
      <tabbar-item path="cart" activeColor = 'deeppink'>
        <template v-slot:item-icon>
          <img src="~assets/img/tabbar/shopcart.svg">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/shopcart_active.svg">
        </template>
        <template v-slot:item-text>
          <div>购物车</div>
        </template>
      </tabbar-item>
      <tabbar-item path="profile" activeColor = 'deeppink'>
        <template v-slot:item-icon>
          <img src="~assets/img/tabbar/profile.svg">
        </template>
        <template v-slot:item-icon-active>
          <img src="~assets/img/tabbar/profile_active.svg">
        </template>
        <template v-slot:item-text>
          <div>个人</div>
        </template>
      </tabbar-item>
    </tab-bar>
  </div>
</template>

<script>
  import TabBar from 'components/common/tabbar/TabBar'
  import TabBarItem from 'components/common/tabbar/TabBarItem'

  export default {
    name: "MainTabBar",
    components: {
      "tab-bar":TabBar,
      "tabbar-item":TabBarItem
    }
  }
</script>

<style scoped>

</style>
