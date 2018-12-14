<template lang="pug">
  div.container.personal-container
    top-image(:top_image="topImage")
    collection
</template>

<script>
import topImage from '../../components/top-image/top-image'
import collection from '../../components/collection/collection'

export default {
  data () {
    return {
      topImage: 'http://pic1.win4000.com/wallpaper/a/599aa3469e7d8.jpg'
    }
  },
  components: {
    topImage,
    collection
  }
}
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"
  .personal-container
    background-color: $backgorund-color
    min-height: 100vh
</style>
