<template>
   <div class="down-footer">
      <div class="container-down-footer">
         <span>SIGN-UP NOW!</span>
         <div class="contacts">
            <span>FOLLOW US</span>
            <ul>
               <li v-for="(item,index) in social" :key="index">
                  <img :src="item.immagine" alt="">
               </li>
            </ul>
         </div>
      </div>
   </div>
</template>
<script>

export default {
   name:'DownFooter',
   data(){
      return {
         social:[
            {
               nome:'facebook',
               link:'',
               immagine:require('../assets/img/footer-facebook.png')
            },
            {
               nome:'twitter',
               link:'',
               immagine:require('../assets/img/footer-twitter.png')
            },
            {
               nome:'youtube',
               link:'',
               immagine:require('../assets/img/footer-youtube.png')
            },
            {
               nome:'pinterest',
               link:'',
               immagine:require('../assets/img/footer-pinterest.png')
            },
            {
               nome:'periscope',
               link:'',
               immagine:require('../assets/img/footer-periscope.png')
            }
         ]
      }
   }
}
</script>
<style lang="scss">
@import '../style/variables.scss';

.down-footer{
   padding: 10px;
   background-color: $dc_darkGrey;
   .container-down-footer{
      @include container_width;
      @include flexy-center;
      justify-content: space-between;
      span{
         border: 1px solid $dc_mainBlue;
         padding: 5px;
         font-size: 0.7em;
         color:$dc_title;
      }
      .contacts{
         @include flexy-center;
         span{
            color:$dc_mainBlue;
            font-weight: bold;
            border: none;
            font-size: 1em;
         }
         ul{
            padding-left: 10px;
            display: flex;
            li{
               list-style-type:none;
               padding: 10px;
               img{
                  max-width: 25px;
               }
            }
         }  
      }
      

   }
}
</style>