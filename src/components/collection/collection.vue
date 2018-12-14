<template lang="pug">
  div.collection-container
    p.title 最近
    div.collection
      div.one-collection(v-for="(item, index) in recent" :key="index")
</template>

<script>
import myTime from '../time/time'

export default {
  data () {
    return {
      recent: [1, 1, 1, 1]
    }
  },
  components: {
    myTime
  }
}
</script>

<style scoped lang="sass" rel="stylesheet/sass">
  @import "~sass/index"
  .collection-container
    display: flex
    flex-direction: column
    align-items: center
    width: 100%
    .title
      margin: 20rpx 0
      font-size: $normal-font-size
      letter-spacing: 3px
    .collection
      display: flex
      flex-wrap: wrap
      justify-content: space-around
      .one-collection
        margin-bottom: 20rpx
        width: 300rpx
        height: 350rpx
        background-color: white
  .de
</style>
