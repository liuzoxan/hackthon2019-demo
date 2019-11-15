<template>
  <div>
    <header-layout></header-layout>
    <section class="shadowbox"></section>
    <div class="main">
      <router-view />
    </div>
  </div>
</template>

<script>
import HeaderLayout from './header'
import './article.less'

export default {
  name: 'Article',
  data() {
    return {}
  },
  components: {
    HeaderLayout
  }
}
</script>
