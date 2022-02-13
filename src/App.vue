<template>
  <div id="app">
    <el-container class="container">
      <el-header class="top">
        <el-menu
          :default-active="activeIndex2"
          class="el-menu-demo"
          mode="horizontal"
          @select="handleSelect"
          background-color="#545c64"
          text-color="#fff"
          active-text-color="#ffd04b"
        >
          <el-menu-item index="1">处理中心</el-menu-item>
          <el-submenu index="2">
            <template slot="title">我的工作台</template>
            <el-menu-item index="2-1">选项1</el-menu-item>
            <el-menu-item index="2-2">选项2</el-menu-item>
            <el-menu-item index="2-3">选项3</el-menu-item>
            <el-submenu index="2-4">
              <template slot="title">选项4</template>
              <el-menu-item index="2-4-1">选项1</el-menu-item>
              <el-menu-item index="2-4-2">选项2</el-menu-item>
              <el-menu-item index="2-4-3">选项3</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-menu-item index="3" disabled>消息中心</el-menu-item>
          <el-menu-item index="4"
            ><a href="https://www.ele.me" target="_blank"
              >订单管理</a
            ></el-menu-item
          >
        </el-menu>
      </el-header>
      <el-container>
        <el-aside class="left">侧边</el-aside>
        <el-main class="content">内容</el-main>
      </el-container>
      <!-- <el-footer class="footer">底部</el-footer> -->
    </el-container>
    <!-- <mainA msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import mainA from './components/mainA.vue'
// import ElementUI from 'element-ui'

// Vue.use(ElementUI);

export default {
  name: "App",
  components: {
    // mainA
  },
  data() {
    return {
      activeIndex: "1",
      activeIndex2: "1",
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
}
.container,
.top,
.left {
  text-align: center;
}
.container {
  width: 100%;
  height: 100vh;
}
.top {
  background: #545c64;
  line-height: 50px;
  color: #fff;
}
.left {
  background: #a1c8ca;
}
.content {
}
</style>
