<template>
  <section :class="templateStyle.content">
    <div :class="templateStyle.rightStyle">
      <p>
        神奇警察
      </p>
      <p>
        <img :src="require('@/assets/policeman.jpg')" />
      </p>
    </div>
  </section>
</template>

<script>
import templateMinix from './templateMinix'
export default {
  mixins: [templateMinix],
  name: 'template3'
}
</script>
