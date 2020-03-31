<template lang="pug">
  el-main.jumbotron
    el-container
      el-main
        h1.title Shop things easily
        h2.subtitle With <strong>tan(t)</strong>, purchase is not what you have to do painfully
        br
        p.subtitle.tight
          i.el-icon-check
          |  Connected to popular stores
        p.subtitle.tight
          i.el-icon-check
          |  Easy access
        p.subtitle.tight
          i.el-icon-check
          |  <i>Odd-yet-satisfying</i> installments
        br
        el-button(type="primary" size="medium" round) See benefits
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({

})
</script>

<style lang="stylus" scoped>
@import "~assets/colors.styl"

.jumbotron
  height 72vh
  background-image url('~static/tantebg-dark.jpg')
  display flex
  align-items center
  background-position center bottom
  background-size cover

.tight
  line-height 1rem
</style>
