<script>
    export default{
        props:{
            image: String,
            title: String,
            price: String,
        }
    }
</script>

<template>
    <div class="comic">
        <img class="immagine_card" :src="image" :alt="title">
        <p style="font-size: 15px; margin-bottom: 0.2rem;">{{ title }}</p>
        <p style="font-size: 15px; margin: 0;">{{ price }}</p>
    </div>
</template>

<style lang="scss" scoped>
    .comic{
        height: 180px;
        width: 180px;
        margin: 1rem;
        .immagine_card{
            width: 100%;
            height: 100%;
        }
    }
</style>

