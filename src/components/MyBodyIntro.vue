<template>
    <div class="container">
        <div class="innerContainer">
            <h2>Music is Life</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem perferendis, aliquam similique, repellendus ut sapiente!</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyBodyIntro'
}
</script>

<style scoped lang="scss">
    .container {
        height: 30vh;
        background-color: #737376;
        display:flex;
        justify-content:center;
        

        .innerContainer {
            width: 50%;
            text-align: center;

            h2 {
                margin: 3rem 3rem;
                color:white;
            };
            p {
                color: white;
            }
        }
    }
</style>