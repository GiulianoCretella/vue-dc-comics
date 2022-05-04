<template>
    <header>
        <div class="logo_container">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li v-for="(item,index) in navList" :key="index">{{item.nome.toUpperCase()}}</li>
            </ul>
        </nav>
    </header>
</template>
<script>
export default {
   name:'appHeader',
   data(){
       return {
           navList:[
               {
                   nome:'characters',
                   active:false,
               },
               {
                   nome:'comics',
                   active:true,
               },
               {
                   nome:'movies',
                   active:false,
               },
               {
                   nome:'tv',
                   active:false,
               },
               {
                   nome:'games',
                   active:false,
               },
               {
                   nome:'collectibles',
                   active:false,
               },
               {
                   nome:'videos',
                   active:false,
               },
               {
                   nome:'fans',
                   active:false,
               },
               {
                   nome:'news',
                   active:false,
               },
               {
                   nome:'shop',
                   active:false,
               }
           ]
       }
   }
}
</script>

<style lang="scss">
@import '../style/variables';

header{
    height: 80px;
    display: flex;
    .logo_container{
        flex: 0 1 35%;
       @include flexy-center;
        img{
            max-width: 60px;
            object-fit: contain;
        }
    }
    nav{
        flex: 1 1 65%;
        @include flexy-center;
        ul{
           @include flexy-center;
           justify-content: space-around;
           
           li{
               list-style-type:none;
               padding: 0 10px;
               font-size: 0.7em;
               font-weight: bolder;
           }
        }
    }
}

</style>