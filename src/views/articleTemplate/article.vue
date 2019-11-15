<template>
  <div>
    <header-layout></header-layout>
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
