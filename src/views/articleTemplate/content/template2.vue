<template>
  <section :class="templateStyle.content">
    <div :class="templateStyle.rightStyle">
      <p>
        互动广告
      </p>
      <p>
        <img :src="require('@/assets/advertising.jpg')" />
      </p>
    </div>
  </section>
</template>

<script>
import templateMinix from './templateMinix'
export default {
  mixins: [templateMinix],
  name: 'template2'
}
</script>
