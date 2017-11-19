<template>
  <v-app>
    <div class="logoBox">
      <div class="logo"></div>
    </div>
  </v-app>
</template>

<style lang="stylus" scoped>
.logoBox
  animation: turn 2s linear forwards 1s
  transform: rotateX(180deg)
  position: relative
  padding: 1rem
  overflow: hidden

.logo
  height: 100px
  width: 100%
  background-image url(~img/clean-logo.svg)
    position: center
    repeat: no-repeat
  overflow: hidden

@keyframes turn
  100%
    transform: rotateX(0deg)

@keyframes godown
  100%
    top: 180px

@keyframes goright
  100%
    left: 70px
</style>
