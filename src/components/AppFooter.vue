<script>
    export default {
        nome: "AppFooter",
        data (){
            return{

            }
        }
    }

</script>

<template>

<footer>
    <div class="big-footer">
        <div class="container flex">
            <div class="lists flex">
                <div>
                    <h5>DC COMICS</h5>
                    <ul>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                        <li>Comics</li>
                    </ul>
    
                    <h5>SHOP</h5>
                    <ul>
                        <li>Shop</li>
                        <li>Shop</li>
                    </ul>
                </div>

                <div>
                    <h5>DC</h5>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                        <li>Terms Of Use</li>
                    </ul>
                </div>

                <div>
                    <h5>SITES</h5>
                    <ul>
                        <li>DC</li>
                        <li>DC</li>
                        <li>DC</li>
                        <li>DC</li>
                        <li>DC</li>
                    </ul>
                </div>

            </div> 

            <div class="dc-logo-bg"></div>
        </div>
    </div>

    <div class="sub-footer">
        <div class="container flex flex-between align-center">
            <div class="btn">SIGN-UP NOW!</div>
    
            <div class="follow-us flex align-center">
                <h4>FOLLOW US</h4>
                <ul class="flex">
                    <li> <a href=""> <img src="../assets/img/footer-facebook.png" alt=""> </a></li>
                    <li> <a href=""> <img src="../assets/img/footer-twitter.png" alt=""> </a></li>
                    <li> <a href=""> <img src="../assets/img/footer-pinterest.png" alt=""> </a></li>
                    <li> <a href=""> <img src="../assets/img/footer-youtube.png" alt=""> </a></li>
                    <li> <a href=""> <img src="../assets/img/footer-periscope.png" alt=""> </a></li>
    
                </ul>
            </div>
        </div>
        
    </div>
</footer>

</template>

<style lang="scss" scoped>
.big-footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .container{
        padding: 0;


        .lists{
            padding: 1rem;
            flex-grow: 1;
            gap: 1.5rem;
            color: white;
    
            h5{
                margin: 0.5rem 0;
            }
        }
    
        .dc-logo-bg{
            flex-grow: 1;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-position: center;
            background-size: cover;
        }
    }

}
.sub-footer{
    background-color: gray;
    .follow-us{

        h4{
            margin-right: 20px;
        }

        ul{
            gap: 20px;
        }
    }
}

</style>