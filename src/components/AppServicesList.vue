<script>


    export default {
        nome: "AppServicesList",
        data (){
            return{
                services: [
                    {
                        name: "digital comics",
                        image: "buy-comics-digital-comics.png",
                    },
                    {
                        name: "dc merchandise",
                        image: "buy-comics-merchandise.png",
                    },
                    {
                        name: "subscription",
                        image: "buy-comics-subscriptions.png",
                    },
                    {
                        name: "comic shop locator",
                        image: "buy-comics-shop-locator.png",
                    },
                    {
                        name: "dc power visa",
                        image: "buy-dc-power-visa.svg",
                    },
                ]

            }   
        },
        methods : {
            getImagePath(url){
                return new URL(url, import.meta.url).href; 
            }
        }
       
    }
</script>

<template>
<div class="services ">
    <div class="container">
        <ul class="flex align-center">
            <li v-for="(item, index) in services" :key="index">
                <div class="flex">
                    <img :src="getImagePath(`../assets/img/${item.image}`)" alt="">
                    <h6> <a href=""> {{item.name}} </a>  </h6>
                </div>
            </li>
        </ul>
    </div>
</div>
</template>

<style lang="scss" scoped>

    .services{
        background-color: #0282F9;
        
        ul{
            justify-content: space-around;

            div{
                align-items: center;


                img{
                    width: 30px;
                    margin-right: 10px;
                }
        
                h6{
                    color: white;
                }
            }
        }
    
    }

    
</style>
