<template lang="pug">
  .container
    el-row(type="flex")
      el-col(:span="16")
        span.footext
          el-link(type="info" @click="openLink") Home
          span.padded |
          el-link(type="info" @click="openLink") About
          span.padded |
          el-link(type="info" @click="openLink") Careers
          span.padded |
          el-link(type="info" @click="openLink") Sitemap
          span.padded |
          el-link(type="info" @click="openLink") Advertise with us!

      el-col.right(:span="8")
        span.footext 2020<sup>&copy;</sup> <i>tan(t)</i> No rights reserved (lul)
</template>

<script lang="ts">
import Vue from 'vue'
import { ElMessageOptions } from 'element-ui/types/message'
export default Vue.extend({
  methods: {
    openLink(): void {
      this.$message({
        message: 'Nah, this just a dummy lul',
        type: 'error',
        duration: 1500,
        showClose: true,
        center: false
      } as ElMessageOptions)
    }
  }
})
</script>

<style lang="stylus" scoped>
@import '~assets/colors.styl'

.container
  position fixed
  bottom 0
  left 0
  width 100vw
  padding 16px

.padded
  padding 0 6px

.right
  display flex
  justify-content flex-end
  text-align right

.footext
  line-height 0.89rem
</style>
