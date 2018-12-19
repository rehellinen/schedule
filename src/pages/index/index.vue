<template lang="pug">
  div.container
    data-time
    my-banner
    alarm-clock
    my-input
</template>

<script>
  import dataTime from '../../components/time/time'
  import myBanner from '../../components/my-banner/my-banner'
  import myInput from '../../components/my-input/my-input'
  import alarmClock from '../../components/alarm-clock/alarm-clock'

  export default {
    components: {
      dataTime,
      myBanner,
      myInput,
      alarmClock
    }
  }
</script>

<style scoped lang="sass">
  @import "~sass/index"
</style>
