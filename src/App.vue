<template>
  <div id="app">
    <app-header/>
    <app-main/>
    <app-footer/>
  </div>
</template>

<script>
import AppFooter from './components/AppFooter.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AppMain,
  }
}
</script>

<style lang="scss">
@import './style/variables.scss';
@import './style/general.scss';


</style>
