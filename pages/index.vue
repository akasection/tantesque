<template lang="pug">
  div
    TanteHeader
    TanteContent
    TanteFooter
</template>

<script lang="ts">
import Vue from 'vue'
import TanteHeader from '~/components/TanteHeader.vue'
import TanteContent from '~/components/TanteContent.vue'
import TanteFooter from '~/components/TanteFooter.vue'

export default Vue.extend({
  components: {
    TanteHeader,
    TanteContent,
    TanteFooter
  },
  methods: {
    goBack(): void {
      console.warn('back')
    }
  }
})
</script>

<style lang="stylus">

</style>
