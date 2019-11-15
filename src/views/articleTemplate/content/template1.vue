<template>
  <section :class="templateStyle.content">
    <div :class="templateStyle.rightStyle">
      <p>
        Autopilot电影
      </p>
      <p>
        <img :src="require('@/assets/movie.png')" />
      </p>
    </div>
  </section>
</template>

<script>
import templateMinix from './templateMinix'
export default {
  mixins: [templateMinix],
  name: 'template1'
}
</script>
