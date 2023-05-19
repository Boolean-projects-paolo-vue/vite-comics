<script>
    
</script>

<template>

    <!-- /***********************************************Parte Blu - Footer***********************************************/ -->

    <section class="blue">
        <div class="container five">
           <ul class="list">
                <li class="point"><img src="./../assets/vue-dc-comics-1/img/buy-comics-digital-comics.png" alt="" class="immagine"><span>DIGITAL COMICS</span></li>
                <li class="point"><img src="./../assets/vue-dc-comics-1/img/buy-comics-merchandise.png" alt="" class="immagine"><span>DC MERCHANDISE</span></li>
                <li class="point"><img src="./../assets/vue-dc-comics-1/img/buy-comics-subscriptions.png" alt="" class="immagine"><span>SUBSCRIPTION</span></li>
                <li class="point"><img src="./../assets/vue-dc-comics-1/img/buy-comics-shop-locator.png" alt="" class="immagine"><span>COMIC SHOP LOCATOR</span></li>
                <li class="point"><img src="./../assets/vue-dc-comics-1/img/buy-dc-power-visa.svg" alt="" class="immagine visa"><span>DC POWER VISA</span></li>
           </ul>
        </div>

    </section>

    <!-- /************************************************Link e Logo - Footer*********************************************/ -->

    <section class="central">
        <div class="container bottom">
            
            <div class="sub-container first_one">
                <div class="alone">
                    <ul>
                        <li><h4 class="title-footer">DC COMICS</h4></li>
                        <li class="punto">Characters</li>
                        <li class="punto">Comics</li>
                        <li class="punto">Movies</li>
                        <li class="punto">TV</li>
                        <li class="punto">Games</li>
                        <li class="punto">Videos</li>
                        <li class="punto">News</li>
                        <li class="punto"><h4 class="title-footer">SHOP</h4></li>
                        <li class="punto">Shop DC</li>
                        <li class="punto">Shop DC Collectibles</li>
                    </ul>
                </div>

                <div class="alone">
                    <ul>
                        <li><h4 class="title-footer">DC</h4></li>
                        <li class="punto">Terms Of Use</li>
                        <li class="punto">Privacy policy (New)</li>
                        <li class="punto">Ad Choises</li>
                        <li class="punto">Advertising</li>
                        <li class="punto">Jobs</li>
                        <li class="punto">Subscription</li>
                        <li class="punto">Talent Workshops</li>
                        <li class="punto">CPSC Certificates</li>
                        <li class="punto">Ratings</li>
                        <li class="punto">Shop Help</li>
                        <li class="punto">Contact Us</li>
                        </ul>
                </div>
                <div class="alone">
                    <ul>
                        <li><h4 class="title-footer">SISTES</h4></li>
                        <li class="punto">DC</li>
                        <li class="punto">MAD Magazine</li>
                        <li class="punto">DC Kids</li>
                        <li class="punto">DC Universe</li>
                        <li class="punto">DC Power Visa</li>
                    </ul>
                </div>
            </div>
            
            <img src="./../assets/vue-dc-comics-1/img/dc-logo-bg.png" alt="" class="img_big">    
        </div>
    </section>

    <!-- /*************************************Sign-up and Follow - Footer*************************************************/ -->

    <section class="bottom_social">
        <div class="socials">
            <button><span class="button_sign">SIGN-UP NOW!</span></button>
            <div class="social-button">
                <h3>FOLLOW US</h3>
                <img src="./../assets/vue-dc-comics-1/img/footer-facebook.png" alt="">
                <img src="./../assets/vue-dc-comics-1/img/footer-twitter.png" alt="">
                <img src="./../assets/vue-dc-comics-1/img/footer-youtube.png" alt="">
                <img src="./../assets/vue-dc-comics-1/img/footer-pinterest.png" alt="">
                <img src="./../assets/vue-dc-comics-1/img/footer-periscope.png" alt="">
            </div>
            </div>
    </section>
</template>

<style lang="scss" scoped>
    @use './../assets/styles/partials/variabels.scss' as *;

    span{
        color: white;
        width: 11rem;
        @include font-arial-600-15
    }
    
    .container{
         max-width: 1450px;
         margin: auto;
    }

    .container.bottom{
        display: flex;
        justify-content: space-between;
        overflow: hidden;
        position: relative;
    }

    .container.five{
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 1.5rem;
    }

    .container.five li{
        margin: 0.5rem;
    }



    .blue{ 
        background-color: rgb(2, 130, 240);
    }
    .list{
        @include my-display-flex-center;
        flex-direction: row;
        height: 100%;
    }
    .point{
        @include my-display-flex-center;
        height: 100%;
    }
    .immagine{
        height: 65px;
        margin: 0.5rem;
        padding: 0.5rem;
    }

    .immagine.visa{
        height: 45px;
    }



    .central{
        background-image: url(./../assets/vue-dc-comics-1/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        font-family: Arial, Helvetica, sans-serif;
    }

    .sub-container.first_one{
        @include my-display-flex-row;
        padding: 2rem;
        height: 80%;
    }
    .alone {
        padding: 1rem;
        height: 80%;
    }
    .title-footer{
        color: white;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 18px;
        margin-bottom: 1rem;
    }
    .punto{
        color: gray;
        margin-bottom: 0.5rem;
        font-size: 12px;
    }

    .img_big{
        position: absolute;
        right: 1rem;
        top: -3rem;
        bottom: 0rem;
    }

    .bottom_social{
    background-color: rgb(48, 48, 48);
    .socials {
        @include flex-align-justify-between;
        max-width: 1350px;
        margin: auto;
        height: 6rem;
        button {
            background-color: transparent;
            color: white;
            border: 2px solid rgb(12, 119, 234);
            padding: 1rem;
            .button_sign{
                font-size: 15px;
            }
        }
        
        .social-button {
            @include my-display-flex-center;
            gap: 1rem;
        }
        h3 {
            color: rgb(12, 119, 234);
            font-family: Arial, Helvetica, sans-serif;
            font-size: 18px;
        }
    }
}

</style>