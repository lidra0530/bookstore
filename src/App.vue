<template>
  <div id="app">
    <el-container>
      <!-- 顶部导航栏 -->
      <div class="topbar">
        <div class="nav">
          <ul>
            <li></li>
            <li>我的订单</li>
            <li>购物车</li>
          </ul>
        </div>
      </div>
      <!-- 顶部导航栏END -->

      <!-- 头部容器 -->
      <el-header> </el-header>
      <!-- 头部容器END -->

      <!-- 主要区域容器 -->
      <el-main>
        <keep-alive>
          <router-view />
        </keep-alive>
      </el-main>
      <!-- 主要区域容器END -->

      <!-- 底部容器 -->
      <el-footer> </el-footer>
      <!-- 底部容器END -->
    </el-container>
  </div>
</template>

<style>
/* 全局样式 */
* {
  padding: 0;
  margin: 0;
  border: 0;
  list-style: none;
}

/* 顶部导航栏样式 */
.topbar {
  height: 40px;
  background-color: #3d3d3d;
  margin-bottom: 20px;
}
.topbar .nav {
  width: 1225px;
  margin: 0 auto;
}
.topbar .nav ul {
  float: right;
}
.topbar .nav li {
  float: left;
  height: 40px;
  color: #b0b0b0;
  font-size: 14px;
  text-align: center;
  line-height: 40px;
  margin-left: 20px;
}
</style>
