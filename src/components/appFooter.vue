<template>
    <footer>
        <up-footer/>
        <central-footer/>
        <down-footer/>
    </footer>
</template>
<script>
import UpFooter from './UpFooter.vue';
import CentralFooter from './CentralFooter.vue';
import DownFooter from './DownFooter.vue';
export default {
   name:'AppFooter',
   components:{
       UpFooter,
       CentralFooter,
       DownFooter,
   }
}
</script>
<style lang="scss">

</style>