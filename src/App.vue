<template>
  <div id="app">
    <header-layout></header-layout>
    <router-view />
  </div>
</template>

<script>
import HeaderLayout from './views/header'
export default {
  name: 'app',
  components: {
    HeaderLayout
  }
}
</script>

<style lang="less" type="text/less">
@import 'style/common.less';
</style>
