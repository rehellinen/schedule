<template lang="pug">
  div.form-container
    form(@submit="formSubmit")
      div.section
        p 输入框：
        textarea(name="name" :value='info')
      div.section
        p 输入框：
        textarea(name="number" :value='info')
      div.section
        p 输入框：
        textarea(name="telephone" :value='info')
      div.section
        p 输入框：
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
    background-color: white
    width: 100%
    form
      display: block
      margin-top: 20rpx
      .section
        border-bottom: 1rpx solid $lighter-font-color
        margin-left: 5%
        width: 90%
        display: flex
        align-items: center
        p
          flex-basis: 20%
          font-size: $small-font-size
          color: $base-font-color
          padding: 20rpx 0 15rpx 0
        textarea
          height: 120rpx
          font-size: $small-font-size
          color: $base-font-color
          padding: 20rpx 0 15rpx 0
      .submit-btn
        width: 89%
        margin: 50rpx 5.4%
        p
          font-size: $normal-font-size
          color: $base-font-color
</style>
