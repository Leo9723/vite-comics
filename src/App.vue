<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import { stringifyExpression } from '@vue/compiler-core';
export default {
  components:{
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>
<template lang="">
  <div>
    <AppHeader></AppHeader>
    <AppMain></AppMain>
    <AppFooter></AppFooter>
  </div>
</template>
<style lang="scss">
  @use './components/styles/general.scss' as *
</style>
