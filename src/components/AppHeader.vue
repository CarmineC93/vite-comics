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
        <div class="container flex flex-between">

            <div class="logo"> 
                <img src="../assets/img/dc-logo.png" alt="logo">
            </div>
            <ul class="flex align-center">
                <li v-for="(link, index) in links"> 
                    <a :href="link.href">{{link.name}}</a>
                </li>
            </ul>

        </div>
    </header>

</template>

<style lang="scss" scoped>

header{
    background-color: white;
    .logo img{
        width: 60px;
    }

    ul{
        gap: 20px;

        a{
            font-size: 0.8rem;
            font-weight: 600;
        }
    }
}




</style>