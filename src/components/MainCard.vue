<template>
    <div class="product-card">
        <div class="card">
             <img :src="thumb" :alt="titolo">
        </div>
             <h3>{{titolo}}</h3>

    </div>
</template>
<script>
export default {
    nome:'ProductCard',
    data(){
        return{

        }

    },
    props:['thumb','titolo']
}
</script>
<style lang="scss" scoped>
@import '../style/variables';

    .product-card{
        width: calc(100% / 6 - 10px);
        padding: 5px;
        margin: 5px;
        .card{
            width: 100%;
            height: 150px;
            overflow: hidden;
            img{
                max-width: 100%;
            }
        }
        h3{
            margin-top: 10px;
            text-align: center;
            font-size: 1em;
            color:$dc_title;
            width: 100%;
        }
    }
</style>