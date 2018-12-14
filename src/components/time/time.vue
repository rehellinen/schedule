<template lang="pug">
  div.time-container
    div
      p.year {{year}}
      p.month-day {{month}} - {{day}}
</template>

<script>
export default {
  created () {
    this._setTime()
  },
  data () {
    return {
      year: 0,
      month: 0,
      day: 0
    }
  },
  methods: {
    _setTime () {
      this.year = new Date().getFullYear()
      this.month = new Date().getMonth() + 1
      this.day = new Date().getDate()
    }
  }
}
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"
  .time-container
    display: flex
    height: 90rpx
    align-items: center
    div
      display: flex
      align-items: baseline
      .year
        font-size: $biggest-font-size
        font-weight: bold
        letter-spacing: 3px
        margin-left: 50rpx
      .month-day
        font-size: $normal-font-size
        margin-left: 20rpx
  .de
</style>
