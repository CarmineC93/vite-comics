<script>
    export default {
        nome: "AppHeader",
        data (){
            return{
                links: [
                    {
                        name: "charaters",
                        href: "/charaters",
                        active: false,
                    },
                    {
                        name: "comics",
                        href: "/comics",
                        active: false,
                    },
                    {
                        name: "movies",
                        href: "/movies",
                        active: false,
                    },
                    {
                        name: "tv",
                        href: "/tv",
                        active: false,
                    },
                    {
                        name: "games",
                        href: "/games",
                        active: false,
                    },
                    {
                        name: "collectibles",
                        href: "/collectibles",
                        active: false,
                    },
                    {
                        name: "videos",
                        href: "/videos",
                        active: false,
                    },
                    {
                        name: "fans",
                        href: "/fans",
                        active: false,
                    },
                    {
                        name: "news",
                        href: "/news",
                        active: false,
                    },
                    {
                        name: "shop",
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
        <div class="container flex flex-between">

            <div class="logo"> 
                <img src="../assets/img/dc-logo.png" alt="logo">
            </div>
            <ul class="flex align-center">
                <li v-for="(link,index) in links"> 
                    <a :href="link.href">{{link.name}}</a>
                </li>
            </ul>

        </div>
    </header>

</template>

<style lang="scss" scoped>
header{
    padding: 1rem;
    // debug
    background-color: pink;

    .logo img{
        width: 60px;
    }

    ul{
        gap: 20px;
    }
}




</style>