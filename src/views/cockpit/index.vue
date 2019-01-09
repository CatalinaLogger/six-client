<template>
  <div class="cockpit-container">
    <img class="map-bg" src="/images/map.svg" alt="">
    <div class="content"></div>
    <block></block>
  </div>
</template>

<script>
import Block from "@/components/block";
export default {
  name: "index",
  components: {
    Block
  }
};
</script>

<style scoped lang="stylus">
.cockpit-container
  position relative
  height 100vh
  background #409EFF
  .map-bg
    width 100%
  .content
    position absolute
    top 0
    width 100%
    height 100%
    opacity .8
    background #1c2145
  .block
    position absolute
    top 0
    z-index 1
</style>
