<template>
    <main>
        <div>
            <span> --> Content goes here </span>
        </div>
    </main>
</template>
<script>
export default {
   name:'AppMain'
}
</script>
<style lang="scss">
    @import '../style/variables.scss';
    main{
        background-color: $dc_ulText_mainDiv;
        height: 80px;
        @include flexy-center;

        div{
            @include container_width;

            span{
            color: $dc_title;
            font-size: 1.2em;
            }
        }
    }
</style>