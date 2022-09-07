<template>
    <div class="card">
        <img class="card-img-top" :src="getImage(imageSrc)" alt="Card image cap">
        <div class="card-body">
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
            return require ('../assets/' + imagePath);
        }
    }
}
</script>

<style scoped lang="scss">
    .card {
        width: 400px;

        .card-body {
            background-color: #4d4d4d;
            padding: 0.5rem;
            
            
            h4 {
                color: #ea4a56;
                font-size: 17px;
            };
            p {
                color: white;
                font-size: 12px;
            }
        }
    }
</style>