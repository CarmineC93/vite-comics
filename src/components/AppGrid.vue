<script>
    export default {
        nome: "AppGrid",
        props: {
            thumb : String,
            price : String,
            series : String,
            type : String
        }

    }
</script>

<template>
    <div class="card">
        <img :src="thumb" :alt="type">
        <h5> <a href="">{{series}}</a>  </h5>
    </div>
</template>

<style lang="scss" scoped>
    .card{
        width: calc(100% / 6 - 10px);
        

        h5{
            margin: 0.8rem;
            color: white;
            text-transform: uppercase;
        }
    }
</style>