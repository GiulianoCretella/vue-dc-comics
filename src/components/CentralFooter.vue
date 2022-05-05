<template>
    <div class="central-footer">
        <div class="container">
            <div class="left-side">
                <ul>
                    <li v-for="(item,index) in footUl" :key="index">{{item.titolo.toUpperCase()}}
                        <ul>
                            <li v-for="(items,index) in footUl[index].sottArray" :key="index">{{items.nome}}</li>
                        </ul>
                    </li>
                </ul>
            </div>
            <div class="right-side">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>
<script>

export default {
   name:'CentralFooter',
   data(){
       return{
           footUl:[
               {titolo: 'dc comics',
                sottArray:[
                    {
                        nome:'Characters',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Comics',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Movies',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'TV',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Games',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Videos',
                        active:false,
                        link:'',
                    },
                    {
                        nome:'News',
                        active:false,
                        link:'',
                    },
                    
                ],
               },
               {titolo: 'dc',
                sottArray:[
                    {
                        nome:'Terms Of Us',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Privacy policy (New)',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Ad Choices',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Advertising',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Jobs',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Subscriptions',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Talent Workshops',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'CPSC Certificates',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Ratings',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Shop Help',
                        active:false,
                        link:'',
                    },
                    {
                        nome:'Contact Us',
                        active:false,
                        link:'',
                    },
                    
                ],
               },
               {titolo: 'sites',
                sottArray:[
                    {
                        nome:'DC',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'MAD Magazine',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'DC Kids',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'DC Universe',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'DC Power Visa',
                        link:'',
                        active:false,
                    },
                ],
               },
               {titolo: 'shop',
                sottArray:[
                    {
                        nome:'Shop DC',
                        link:'',
                        active:false,
                    },
                    {
                        nome:'Shop SC Collectables',
                        link:'',
                        active:false,
                    },
                ],
               }
               
           ]
       }
   }
}
</script>
<style lang="scss">
@import '../style/variables.scss';
.central-footer{
    background-image:url(../assets/img/footer-bg.jpg);
    background-size:cover;
    .container{
        @include container_width;
        @include flexy-center;
        height: 400px;
        .left-side{
            @include flexy-center;
            flex: 0 1 50%;
            justify-content: flex-start;
            ul{
                display: flex;
                flex-flow: wrap;
                li{
                    list-style-type: none;
                    color:$dc_title;
                    margin: 10px;
                    font-size: 1em;
                    font-weight: bold;
                    ul{
                        display: block;
                        li{
                            color:$dc_lightGrey;
                            margin:5px 0;
                            font-size: 0.7em;
                        }
                    }
                }
            }
        }
        .right-side{
            flex: 0 1 50%;
            overflow:hidden;
            height: 100%;
        }
    }
}
</style>