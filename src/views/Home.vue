<template>
  <div class="home">
    <el-container>
      <el-header>
        <div class="logo">
          <img src="@/assets/logo.png" />
          <h1 class="logo-text">Vue2.0 TypeScript</h1>
        </div>
      </el-header>
      <el-container>
        <el-aside width="200px">Aside</el-aside>
        <el-main>Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Provide } from "vue-property-decorator";
@Component({
  components: {},
})
export default class Home extends Vue {
  // @Provide() logoImg = require('../assets/')
}
</script>

<style lang="scss">
.home {
  height: 100%;
}
.el-header {
  background-color: #001529;
  line-height: 60px;
}
.logo {
  display: flex;
  align-items: center;
  img {
    width: 30px;
    height: 30px;
  }
  .logo-text {
    color: #fff;
    margin-left: 10px;
    font-size: 18px;
  }
}
.el-aside {
  background-color: #d3dce6;
  height: calc(100vh - 60px);
}

.el-main {
  background-color: #e9eef3;
  min-width: 500px;
}
</style>