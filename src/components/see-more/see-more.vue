<template lang="pug">
div.more-container
  p {{text}}
  img(src="/static/images/icon/arrow@downBlack.png")
</template>

<script>
  export default {
    props: {
      text: {
        type: String,
        default: '查看更多'
      }
    }
  }
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"
  .more-container
    width: 100%
    display: flex
    justify-content: flex-end
    align-items: center
    color: $light-font-color
    height: 65rpx
    background-color: white
    margin-bottom: 5rpx
    p
      font-size: $small-font-size
    img
      transform: rotate(270deg)
      height: 40rpx
      width: 40rpx
      margin-right: 10rpx
</style>
