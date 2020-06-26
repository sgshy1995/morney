<template>
  <div class="app">
    <el-row type="flex" justify="center">
      <el-col :span="8">
        <router-link to="/money">首页</router-link>
      </el-col>
      <el-col :span="8">
        <router-link to="/labels">标签</router-link>
      </el-col>
      <el-col :span="8">
        <router-link to="statistics">统计</router-link>
      </el-col>
    </el-row>
  </div>
</template>

<script lang="ts">
  import Vue from 'vue';
  import {Component} from 'vue-property-decorator';

  @Component
  export default class Nav extends Vue {

  }
</script>

<style scoped lang="scss">
  .app {
    height: 100%;
  }

  .el-row {
    height: 100%;
  }

  .el-col {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
  }

</style>