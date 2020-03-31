<template lang="pug">
  .header
    el-row(type="flex" style="padding: 0 16px")
      el-col(:span="4" class="logo-col")
        el-image(
          :src="require('~/static/tante-logotype.png')"
          alt="logo"
          :z-index="1"
          fit="contain"
          style="height: 36px")
      el-col(:span="14")
      el-col(:span="6" class="action-col")
        el-button(type="success" disabled) Signup
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({

})
</script>

<style lang="stylus" scoped>
@import "~assets/colors.styl"

.header
  width 100vw
  position sticky
  top 0
  left 0
  background-color color-secondary
  padding-top 12px
  padding-bottom 12px
  box-shadow 0 2px 6px 0px #0000003b

.action-col
  display flex
  justify-content flex-end

.logo-col
  display flex
  justify-content flex-start
</style>
