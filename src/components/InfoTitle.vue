<template>
    <div class="innerContainer">
        <h2>{{title}}</h2>
        <hr>
        <p>{{paragraph}}</p>
    </div>
</template>

<script>
export default {
    name: 'InfoTitle',
    props: {
        info: Array
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