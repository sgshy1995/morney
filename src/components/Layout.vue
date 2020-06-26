<template>
  <div>
    <el-container>
      <el-main>
        <slot></slot>
      </el-main>
      <el-footer>
        <Nav></Nav>
      </el-footer>
    </el-container>
  </div>
</template>

<script lang="ts">
  import Vue from 'vue';
  import {Component} from 'vue-property-decorator';

  @Component
  export default class Layout extends Vue {

  }
</script>

<style scoped lang="scss">
  .el-container{
    height: 100vh;
  }
  .el-main{
    overflow: auto;
    padding: 0;
  }
  .el-footer{
    padding: 0;
    border: 1px solid black;
  }
</style>