<template>
  <div class="main">
    <section class="demo">
      <div class="demo__title">基础用法</div>
      <swiper
        autoplay
        circular
        indicator-dots
        indicator-active-color="#f60"
        class="swiper"
      > 
        <swiper-item class="swiper__item" v-for="i in 4" :key="i">
          <img class="img" src="/static/demo/2.jpeg"/>
        </swiper-item>
      </swiper>
    </section>


    <section class="demo">
      <div class="demo__title">垂直滚动</div>
      <swiper
        autoplay
        circular
        indicator-dots
        indicator-active-color="#f60"
        vertical
        class="swiper"
      > 
        <swiper-item class="swiper__item" v-for="i in 4" :key="i">
          <img class="img" src="/static/demo/2.jpeg"/>
        </swiper-item>
      </swiper>
    </section>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  },
  methods: {}
}
</script>

<style scoped src="css-utils-collection"></style>
<style scoped src="@/assets/demo.css"></style>
<style scoped>
.swiper {
  height: 100px;
}
.swiper__item {
  display: flex;
  justify-content: center;
}
.swiper .img {
  max-width: 100%;
  max-height: 100%;
}

</style>
