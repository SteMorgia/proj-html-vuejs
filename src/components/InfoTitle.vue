<template>
    <div class="innerContainer">
        <h2>{{titolo}}</h2>
        <hr>
        <p>{{paragrafo}}</p>
    </div>
</template>

<script>
export default {
    name: 'InfoTitle',
    props: {
        titolo: String,
        paragrafo: String
    }
}
</script>

<style scoped lang="scss">
        
    .innerContainer {
        text-align: center;
        width: 50%;
        display:flex;
        flex-direction: column;
        align-items: center;

        h2 {
            padding-top: 3rem;
            margin-bottom: 1rem;
            color:white;
        };
        hr {
            width:50%;
            text-align: center;
        }
        p {
            color: white;
            padding-top: 1rem;
        }
    }
    
</style>