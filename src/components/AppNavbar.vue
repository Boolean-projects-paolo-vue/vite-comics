<script>
    export default{
        props:{
            title: String,
            link: String,
        }
    }
</script>

<template>
    <div class="dflex">
        <div class="point"> {{ title }}
            <div class="line" style="border: 3px solid rgb(12, 119, 234); margin: 0.5rem;"></div>
        </div> 
          
    </div>
       
</template>

<style lang="scss" scoped>
    @use './../assets/styles/partials/variabels.scss' as *;

    .dflex{
        position: relative;
    }

    .point{
        font-weight: 700;
        margin: 0.5rem;

        &:hover{
            cursor: pointer;
            color:rgb(12, 119, 234);
        };
        &:hover .line{
            display: block;
        }
    }


    .line{
        display: none;
        position: absolute;
        width: 100%;
        bottom: 0rem;
        top: 3.7rem;
        left: -0.5rem; 
    }

    /*li.active::after {
        content: "";
        display: block;
        width: 50px;
        height: 5px;
        background-color: #0282f9;
        position: absolute;
        top: 65px;
        left: 7px;
    }*/
    
</style>