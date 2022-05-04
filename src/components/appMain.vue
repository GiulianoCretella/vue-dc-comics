<template>
    <main>
        <span> --> Content goes here </span>
    </main>
</template>
<script>
export default {
   name:'appMain'
}
</script>
<style lang="scss">
    @import '../style/variables.scss';
    main{
        background-color: $dc_ulText_mainDiv;
        height: 80px;

        span{
            color: $dc_title;
        }
    }
</style>