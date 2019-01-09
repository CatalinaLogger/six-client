<template>
  <div class="block">
    <div class="master">
      <div class="progress">
        <i class="icon-uniE900 a"></i>
        <i class="icon-uniE900 b"></i>
        <i class="icon-uniE900 c"></i>
        <i class="icon-uniE900 d"></i>
        <i class="icon-uniE900 e"></i>
      </div>
    </div>
    <div class="corner left-top"></div>
    <div class="corner right-top"></div>
    <div class="corner right-bottom"></div>
    <div class="corner left-bottom"></div>
  </div>
</template>

<script>
export default {
  name: "index"
};
</script>

<style scoped lang="stylus">
$borderSize=6px
@keyframes running
  0%
    color white
  50%
    font-size 22px
    color rgba(255, 255, 255, 0)
  100%
    color white
.progress
  padding 20px
  font-size 28px
  color rgba(255, 255, 255, 0)
  .a
    animation running 2s infinite .5s linear
  .b
    animation running 2s infinite .4s linear
  .c
    animation running 2s infinite .3s linear
  .d
    animation running 2s infinite .2s linear
  .e
    animation running 2s infinite .1s linear
.block
  margin 50px
  position relative
  width 400px
  height 400px
  .master
    width 100%
    height 100%
    border $borderSize solid #30378e
    box-shadow inset 0 0 20px #30378e
    box-shadow 0 0 20px #ffffff
  .corner
    position absolute
    width 40px
    height 40px
    &.left-top
      top 0
      border-left $borderSize solid white
      border-top $borderSize solid white
    &.right-top
      top 0
      right 0
      border-top $borderSize solid white
      border-right $borderSize solid white
    &.right-bottom
      right 0
      bottom 0
      border-right $borderSize solid white
      border-bottom $borderSize solid white
    &.left-bottom
      bottom 0
      border-left $borderSize solid white
      border-bottom $borderSize solid white
</style>
