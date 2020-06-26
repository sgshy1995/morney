<template>
  <div>
    <div>访问页面不存在，请检查路径</div>
    <router-link to="/">返回首页</router-link>
  </div>
</template>

<script lang="ts">
  import Vue from 'vue';
  import {Component} from 'vue-property-decorator';

  @Component
  export default class NotFound extends Vue {

  }
</script>

<style scoped lang="scss">

</style>