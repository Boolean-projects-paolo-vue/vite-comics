<script>
    
</script>

<template>
        <div class="container">
            <div class="sub-container">
                <div>
                    <img src="./../assets/vue-dc-comics-1/img/dc-logo.png" alt="" class="logo">
                </div>
                <div>
                    <ul class="list">
                        <li>CHARACTERS</li>
                        <li>COMICS</li>
                        <li>MOVIES</li>
                        <li>TV</li>
                        <li>GAMES</li>
                        <li>COLLECTIBES</li>
                        <li>VIDEOS</li>
                        <li>FANS</li>
                        <li>NEWS</li>
                        <li>SHOP</li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="jumbo">

        </div>
    
</template>

<style lang="scss" scoped>
@use './../assets/styles/partials/variabels.scss' as *;  

    .container{
        background-color: white;
    }

    .sub-container{
        height: 7rem;
        max-width: 1350px;
        margin: auto;
        @include my-display-flex-between;
        @include font-arial-600-15;
    }

    .container .sub-container li{
        padding: 0.5rem;
    }
    .jumbo{
        background-image: url(./../assets/vue-dc-comics-1/img/jumbotron.jpg);
        height: 25rem;
    }

    .logo{
        height: 65px;
    }
    .list{
        @include my-display-flex-row;

        li{
            &:hover{
                cursor: pointer;
                color:blue
            };
        }
    }
</style>