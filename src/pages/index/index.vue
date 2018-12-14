<template lang="pug">
  div.container
    data-time
    wux-button 5555
</template>

<script>
  import dataTime from '../../components/time/time'

  export default {
    components: {
      dataTime
    }
  }
</script>

<style scoped lang="sass">
  @import "~sass/index"
</style>
