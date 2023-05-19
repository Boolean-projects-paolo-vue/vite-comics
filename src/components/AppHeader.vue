<script>
    import AppNavbar from './AppNavbar.vue'
    export default{
        components:{
            AppNavbar,
        },
        data() {
            return {
                ArrayHarder: [
                    {
                        title: 'CHARACTERS',
                        link:"#",
                    },
                    {
                        title: 'COMICS',
                        link:"#",
                    },
                    {
                        title: 'MOVIES',
                        link:"#",
                    },
                    {
                        title: 'TV',
                        link:"#",
                    },
                    {
                        title: 'GAMES',
                        link:"#",
                    },
                    {
                        title: 'COLLECTIBES',
                        link:"#",
                    },
                    {
                        title: 'VIDEOS',
                        link:"#",
                    },
                    {
                        title: 'FANS',
                        link:"#",
                    },
                    {
                        title: 'NEWS',
                        link:"#",
                    },
                    {
                        title: 'SHOP',
                        link:"#",
                    },
                ],
            };
        },
    };
</script>

<template>
    <section>
        <div class="container">
            <div class="sub-container">
                <div>
                    <img src="./../assets/vue-dc-comics-1/img/dc-logo.png" alt="" class="logo">
                </div>
                <div>
                    <ul class="list">
                        <AppNavbar 
                            v-for="index in ArrayHarder" 
                            :key="index.title"
                            :title="index.title"
                            :link="index.link"
                        />
                    </ul>   
                </div>
            </div>
        </div>
        <div class="jumbo">
            <button class=" button_series"><a href="">CURRENT SERIES</a></button>
        </div>
    </section>
        
    
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

    .logo{
        height: 65px;
    }
    
    .list{
        @include my-display-flex-row;
    }

    .jumbo{
        background-image: url(./../assets/vue-dc-comics-1/img/jumbotron.jpg);
        background-size: cover;
        height: 25rem;
        position: relative;
    }

    .button_series{
        padding-inline: 1.5rem;
        padding-top: 0.3rem;
        padding-bottom: 0.3rem;
        position:absolute;
        left: 20rem;
        bottom: -1.5rem;
        background-color: rgb(12, 119, 234);
        font-size: 20px ;
        font-weight: 600;
        color:white;
        border: 0;
        a{
            text-decoration: none;
            color: white;
        }
       
    }

    
    
</style>