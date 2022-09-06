<template>
    <div class="card">
        <img :src="getImage(imageSrc)" />
        <div class="container">
            <h4>{{titolo}}</h4> 
            <p>{{paragrafo}}</p> 
        </div>
    </div>
</template>

<script>
export default {
    name: 'SingleCard',
    props: {
        imageSrc: String,
        titolo: String,
        paragrafo: String
    },
    methods: {
        getImage(imagePath) {
            return require (imagePath);
        }
    }
}
</script>

<style scoped lang="scss">
    
</style>