<template>
    <div class="up-footer">
        <div class="card-container">
            <ul>
                <li v-for="(item,index) in shopList" :key="index">
                    <img :src="item.immagine" alt="">
                    <span>{{item.testo.toUpperCase()}}</span>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>

export default {
   name:'UpFooter',
   data(){
       return{
           shopList:[
               {
                   immagine:require("../assets/img/buy-comics-digital-comics.png"),
                   testo:'digital comics',
               },
               {
                   immagine:require('../assets/img/buy-comics-merchandise.png'),
                   testo:'dc merchandise',
               },
               {
                   
                   immagine:require('../assets/img/buy-comics-subscriptions.png'),
                   testo:'subscription',
               },
               {
                   immagine:require('../assets/img/buy-comics-shop-locator.png'),
                   testo:'comic shop location',
               },
               {
                   immagine:require('../assets/img/buy-dc-power-visa.svg'),
                   testo:'dc power visa',
               }
           ]
       }
   }
}
</script>
<style lang="scss">
    @import '../style/variables.scss';
    div.up-footer{
        background-color:$dc_mainBlue;
        .card-container{
            @include container_width;
            height: 100%;
            padding: 10px 0;
            ul{
               display: flex;
               li{
                   @include flexy-center;
                   padding:15px;
                   list-style-type: none;
                   width: calc(100% / 5);
                   img{
                       max-width: 30px;
                   }
                   span{
                       color: $dc_title;
                       font-size: 0.6em;
                       margin-left: 5px
                   }
               }
            }
        }

    };
</style>