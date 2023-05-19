<script>
    export default{
        props:{
            image: String,
            name: String,
            price: String,

        }
    }
</script>

<template>
    <div class="comic">
        <img :src="image" :alt="card.series">
        <h2>{{ name }}</h2>
        <p>{{ price }}</p>
    </div>
</template>

<style lang="scss" scoped>
    
</style>

