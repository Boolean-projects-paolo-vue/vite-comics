<script>
    export default{
        props:{
            title: String,
            link: String,
        }
    }
</script>

<template>
        <li class="point"> {{ title }}</li>  
</template>

<style lang="scss" scoped>
    @use './../assets/styles/partials/variabels.scss' as *;

    

    .point{
        font-weight: 700;
        &:hover{
            cursor: pointer;
            color:rgb(12, 119, 234);
        };
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