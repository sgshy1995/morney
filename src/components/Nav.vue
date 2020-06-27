<template>
  <div class="app">
    <el-row type="flex" justify="center">
      <el-col :span="8">
        <router-link to="/money" class="wrapper">
          <i class="el-icon-mobile icon"></i>
          <span>记账</span>
        </router-link>
      </el-col>
      <el-col :span="8">
        <router-link to="/labels" class="wrapper">
          <i class="el-icon-collection-tag icon"></i>
          <span>标签</span>
        </router-link>
      </el-col>
      <el-col :span="8">
        <router-link to="statistics" class="wrapper">
          <i class="el-icon-notebook-2 icon"></i>
          <span>统计</span>
        </router-link>
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
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100%;
  }
  .wrapper{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-decoration: none;
    color: inherit;
    font-size: 14px;
    border: 1px solid black;
    padding: 5px 20px;
    border-radius: 5px;
  }
  .wrapper:focus{
    color: red;
    border-color: red;
  }

  .icon{
    width: 1em;
    height: 1em;
  }

</style>