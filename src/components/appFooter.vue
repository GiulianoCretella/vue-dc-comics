<template>
    <footer>
        <up-footer/>
        <central-footer/>
        <down-footer/>
    </footer>
</template>
<script>
import upFooter from './upFooter.vue';
import centralFooter from './centralFooter.vue';
import downFooter from './downFooter.vue';
export default {
   name:'appFooter',
   components:{
       upFooter,
       centralFooter,
       downFooter,
   }
}
</script>
<style lang="scss">

</style>