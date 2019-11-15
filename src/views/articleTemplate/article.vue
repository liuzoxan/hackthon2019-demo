<template>
  <div>
    <header-layout></header-layout>
    <div>
      <router-view />
    </div>
  </div>
</template>

<script>
import HeaderLayout from './header'

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
