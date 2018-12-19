<template lang="pug">
  div.form-container
    p.title 管理工作
    form(@submit="formSubmit")
      div.section
        img(src="/static/images/theme/input@one.jpg" mode="aspectFill")
        p 重要而紧急的工作：
        textarea(name="name" :value='info')
      div.section
        img(src="/static/images/theme/input@two.jpg" mode="aspectFill")
        p 重要而不紧急的工作：
          textarea(name="number" :value='info')
      div.section
        img(src="/static/images/theme/input@three.jpg" mode="aspectFill")
        p 紧急而不重要的工作：
        textarea(name="telephone" :value='info')
      div.section
        img(src="/static/images/theme/input@four.jpg" mode="aspectFill")
        p 一般的工作：
        textarea(name="weixin" :value='info')
      div.title-section
        p.title 管理感悟
      div.section
        textarea(name="weixin" :value='info')
      button.submit-btn(formType="submit")
        p 提交
</template>

<script>
export default {

}
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"

  .form-container
    display: flex
    flex-direction: column
    align-items: center
    background-color: $backgorund-color
    width: 100%
    .title
      margin: 20rpx 0
      font-size: $normal-font-size
      letter-spacing: 3px
    form
      .title-section
        display: flex
        justify-content: center
        p
          margin-top: 0

      .section
        background-color: white
        border-radius: 10px
        box-sizing: border-box
        margin-bottom: 20rpx
        padding: 0 20rpx
        height: 210rpx
        width: 710rpx
        display: flex
        flex-direction: column
        img
          position: absolute
          left: 20rpx
          border-radius: 10px
          width: 710rpx
          height: 210rpx
        p
          font-size: $small-font-size
          color: $base-font-color
          padding: 20rpx 0 15rpx 0
          z-index: 10
        textarea
          width: 100%
          height: 100rpx
          font-size: $small-font-size
          color: $base-font-color
          margin: 20rpx 0
          border-bottom: 1px solid  $lighter-font-color
          z-index: 10
      .section:last-child
        height: 350rpx
        textarea
          height: 350rpx
      .submit-btn
        width: 710rpx
        margin: 0 auto 20rpx
        p
          font-size: $normal-font-size
          color: $base-font-color
</style>
