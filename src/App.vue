<template>
  <el-container>
    <el-header>Header</el-header>
    <el-container>
      <el-aside width="200px">
        <el-row>
          <el-menu
            default-active="2"
          >
            <el-menu-item index="0">
              <i class="el-icon-menu"></i>
              <router-link to="/">Home</router-link>
            </el-menu-item>
            <el-menu-item index="1">
              <i class="el-icon-menu"></i>
              <router-link to="/about">About</router-link>
            </el-menu-item>
          </el-menu>
        </el-row>
      </el-aside>
      <el-main>
        <router-view/>
      </el-main>
    </el-container>
  </el-container>
</template>

<style lang="scss">
  .el-header {
    background-color: #B3C0D1;
    color: #333;
    line-height: 60px;
  }
  
  .el-aside {
    background-color: #D3DCE6;
    color: #333;
  }
  
  .el-main {
    background-color: #E9EEF3;
    color: #333;
  }
</style>
