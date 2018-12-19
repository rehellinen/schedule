<template lang="pug">
  div
    div.clock-container
      div.left
        img(src="/static/images/icon/clock.png")
        p 日程
      div.reminder
        div.time-container
          p.comment 早上
          p.time 9:00
        p.todo 会议
    see-more
</template>

<script>
  import seeMore from '../see-more/see-more'
  export default {
    components: {
      seeMore
    }
  }
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"
  .clock-container
    display: flex
    flex-direction: column
    padding-top: 25rpx
    .left
      display: flex
      width: 160rpx
      align-items: center
      justify-content: center
      border-right: 1px solid $lighter-font-color
      margin-bottom: 20rpx
      img
        width: 40rpx
        height: 40rpx
      p
        font-size: $small-font-size
        color: $light-font-color
        margin-left: 20rpx
    .reminder
      display: flex
      margin: 10rpx 20rpx
      .time-container
        display: flex
        align-items: baseline
        .comment
          font-size: $small-font-size
          color: $light-font-color
        .time
          font-size: $big-font-size
          margin-left: 15rpx
      .todo
        font-size: $normal-font-size
        flex: 1
        margin-left: 40rpx
        border-bottom: 1px solid $light-font-color
    .de
</style>
