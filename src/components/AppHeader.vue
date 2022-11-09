<script>
    export default {
        nome: "AppHeader",
        data (){
            return{
                links: [
                    {
                        name: "CHARACTHERS",
                        href: "/characters",
                        active: false,
                    },
                    {
                        name: "COMICS",
                        href: "/comics",
                        active: false,
                    },
                    {
                        name: "MOVIES",
                        href: "/movies",
                        active: false,
                    },
                    {
                        name: "TV",
                        href: "/tv",
                        active: false,
                    },
                    {
                        name: "GAMES",
                        href: "/games",
                        active: false,
                    },
                    {
                        name: "COLLECTIBLES",
                        href: "/collectibles",
                        active: false,
                    },
                    {
                        name: "VIDEOS",
                        href: "/videos",
                        active: false,
                    },
                    {
                        name: "FANS",
                        href: "/fans",
                        active: false,
                    },
                    {
                        name: "NEWS",
                        href: "/news",
                        active: false,
                    },
                    {
                        name: "SHOP",
                        href: "/shop",
                        active: false,
                    },
                ]
            }

        }
    }
</script>

<template>
    <header>
        <nav class="container flex flex-between">

            <div class="logo"> 
                <a href="">
                    <img src="../assets/img/dc-logo.png" alt="logo">
                </a> 
                
            </div>
            <ul class="flex align-center">
                <li v-for="(link, index) in links" :key="index"> 
                    <a :href="link.href">{{link.name}}</a>
                </li>
            </ul>

        </nav>
    </header>

</template>

<style lang="scss" scoped>

header{
    background-color: white;
    line-height: 60px;
    .container{
        padding: 0 1rem 0 1rem;
    
        .logo img{
            width: 60px;
            vertical-align: middle;
            margin: 1rem 0;

        }

        ul{
            gap: 20px;

            a{
                font-size: 0.8rem;
                font-weight: 600;
                display: inline-block;
                line-height: inherit;
            }
        }
    }
}




</style>