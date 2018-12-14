<template lang="pug">
  div.banner-container
    swiper.banner(interval='5000', :indicator-dots='true', :autoplay='true')
      swiper-item(v-for="(item, index) in banner", :key="index")
        div.text
          p 生活就像海洋，只有意志坚强才能达到彼岸
        div.shadow
        img(:src="item")
</template>

<script>
export default {
  data () {
    return {
      banner: [
        'http://pic1.win4000.com/wallpaper/a/599aa3469e7d8.jpg',
        'http://pic1.win4000.com/wallpaper/a/599aa3469e7d8.jpg'
      ]
    }
  }
}
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"
  .banner-container
    width: 100%
    swiper
      width: 100%
      height: 400rpx
      .text
        display: flex
        justify-content: center
        align-items: center
        width: 100%
        height: 95%
        position: absolute
        top: 0
        z-index: 100
        p
          font-size: $big-font-size
          letter-spacing: 1px
          width: 80%
          color: white
      .shadow
        background-color: #000
        opacity: 0.5
        width: 100%
        height: 100%
        position: absolute
        top: 0
      img
        width: 100%
        height: 100%
  .de
</style>
