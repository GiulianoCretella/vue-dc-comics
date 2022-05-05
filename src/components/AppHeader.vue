<template>
    <header>
        <div class="header-container">
            <div class="logo_container">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav>
                <ul>
                    <li v-for="(item,index) in navList" :key="index" :class="{'selected' : item.active}" @click="item.active = true">{{item.nome.toUpperCase()}}</li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script>

export default {
   name:'AppHeader',
   data(){
       return {
           navList:[
               {
                   nome:'characters',
                   active:false,
                   link:'',
               },
               {
                   nome:'comics',
                   link:'',
                   active:true,
               },
               {
                   nome:'movies',
                   link:'',
                   active:false,
               },
               {
                   nome:'tv',
                   link:'',
                   active:false,
               },
               {
                   nome:'games',
                   link:'',
                   active:false,
               },
               {
                   nome:'collectibles',
                   link:'',
                   active:false,
               },
               {
                   nome:'videos',
                   active:false,
                   link:'',
               },
               {
                   nome:'fans',
                   link:'',
                   active:false,
               },
               {
                   nome:'news',
                   link:'',
                   active:false,
               },
               {
                   nome:'shop',
                   link:'',
                   active:false,
               }
           ]
       }
   },
   methods:{
      seleziona(){
          
      }
   }
}
</script>

<style lang="scss">
@import '../style/variables';
header{
    background-color: white;
    .header-container{
        height: 80px;
        display: flex;
        @include container_width;
        .logo_container{
            flex: 0 1 40%;
        @include flexy-center;
        justify-content: flex-start;
            img{
                max-width: 60px;
                object-fit: contain;
            }
        }
        nav{
            flex: 0 1 60%;
            @include flexy-center;
            justify-content: flex-end;
            ul{
            @include flexy-center;
            li{
                list-style-type:none;
                padding:0 10px;
                font-size: 0.7em;
                font-weight: bolder;
                line-height: 76px;
                border-bottom: 4px solid white;
            }
            }
        }
        .selected{
            border-bottom: 4px solid $dc_mainBlue;
        }
    }
}

</style>