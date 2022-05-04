<template>
  <div id="app">
    <app-header/>
    <app-main/>
    <app-footer/>
  </div>
</template>

<script>
import appFooter from './components/appFooter.vue'
import appHeader from './components/appHeader.vue'
import appMain from './components/appMain.vue'

export default {
  name: 'App',
  components: {
    appHeader,
    appFooter,
    appMain,
  }
}
</script>

<style lang="scss">

</style>
