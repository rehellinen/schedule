<template lang="pug">
  div.container
    data-time
    my-banner
    my-input
</template>

<script>
  import dataTime from '../../components/time/time'
  import myBanner from '../../components/my-banner/my-banner'
  import myInput from '../../components/my-input/my-input'

  export default {
    components: {
      dataTime,
      myBanner,
      myInput
    }
  }
</script>

<style scoped lang="sass">
  @import "~sass/index"
</style>
