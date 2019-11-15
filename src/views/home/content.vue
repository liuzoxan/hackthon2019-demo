<template>
  <div class="home">
    <section class="title">
      <img v-bind:src="logoUrl" />
      <p>" Feel your feeling "</p>
      <h1>
        <span class="slogan1">真实.</span><span class="slogan2">互动.</span
        ><span class="slogan3">有趣.</span>
      </h1>
    </section>
    <div class="wrapper">
      <section class="container">
        <ul class="ulStyle">
          <li v-for="(item, index) in articleData" :key="index" class="liStyle">
            <div class="picture">
              <img :src="item.imgSrc" />
            </div>
            <router-link :to="item.link" class="textStyle">
              {{ item.text }}
            </router-link>
          </li>
        </ul>
      </section>
    </div>
  </div>
</template>

<script>
import './content.less'
export default {
  name: 'Content',
  data() {
    return {
      logoUrl: require('@/assets/logo_dark.png'),
      articleData: [
        {
          imgSrc: require('@/assets/movie.png'),
          text: 'Autopilot电影：有趣的情感互动电影，体验属于你自己的电影',
          link: { name: 'Template1' }
        },
        {
          imgSrc: require('@/assets/advertising.jpg'),
          text: '互动广告：立体情景追踪，陪伴你的信息小管家',
          link: { name: 'Template2' }
        },
        {
          imgSrc: require('@/assets/policeman.jpg'),
          text: '神奇警察：可疑敲门人，家庭安保员',
          link: { name: 'Template3' }
        }
      ]
    }
  }
}
</script>
