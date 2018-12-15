<template lang="pug">
div.info-container
  img.header-image(:src="top_image")
  open-data.avatar-name(type="userNickName", v-if="type === 'user'")
  open-data.avatar(type="userAvatarUrl", v-if="type === 'user'")
  img.avatar(:src="avatar", v-if="type !== 'user'")
  p.avatar-name(v-if="type !== 'user'") {{name}}
  div.info
    div
      img(src="/static/images/icon/info.png")
      p.text 关于我们
    div
      p.count 30
      p.text 我的收藏
</template>

<script>
  export default {
    props: {
      top_image: {
        type: String,
        default: '__IMAGE__/theme/personal@header.jpg'
      },
      avatar: {
        type: String,
        default: '__IMAGE__/theme/personal@avatar.jpg'
      },
      name: {
        type: String,
        default: 'tuntematon'
      },
      quote: {
        type: String,
        default: '生活就像海洋，只有意志坚强的人才能到达彼岸'
      },
      type: {
        type: String,
        default: 'user'
      }
    }
  }
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"

  .info-container
    display: flex
    flex-direction: column
    align-items: center
    background-color: white
    position: relative
    .header-image
      width: 750rpx
      height: 325rpx
    .avatar
      width: 150rpx
      height: 150rpx
      position: absolute
      top: 250rpx
      border-radius: 50%
      display: block
      overflow: hidden
    .avatar-name
      margin-top: 85rpx
      color: $base-font-color
      letter-spacing: 2px
      font-size: $bigger-font-size
    .info
      display: flex
      width: 100%
      justify-content: space-between
      margin: 30rpx 0 15rpx 0
      height: 90rpx
      div
        height: 100%
        display: flex
        flex-direction: column
        justify-content: space-between
        align-items: center
        margin: 0 70rpx
        img
          width: 30rpx
          height: 30rpx
        .count
          font-size: $normal-font-size
        .text
          font-size: $small-font-size
          color: $light-font-color
  .desc-class
</style>
