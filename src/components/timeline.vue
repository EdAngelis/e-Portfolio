<template lang='pug'>
  v-container(justify-center)
    div#timeline-line(justify-center)
</template>

<script>
export default {
  name: 'timeline',
  }
</script>

<style scoped>
#timeline-line{
    position: absolute;
    left: 50%;
    background-color: red;
    width: 3px;
    height: 1000px;
}
</style>