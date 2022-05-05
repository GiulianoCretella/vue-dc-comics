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
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
@import './style/variables.scss';
@import './style/general.scss';
body{
  font-family: 'Roboto', sans-serif;
}


</style>
