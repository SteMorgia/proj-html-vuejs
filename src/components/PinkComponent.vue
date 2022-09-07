<template>
    <div class="pinkContainer">
        <p>{{paragrafo}}</p>
    </div>
</template>

<script>
export default {
    name: 'PinkComponent',
    props: {
        paragrafo: String
    }
}
</script>

<style scoped lang="scss">
    .pinkContainer {
        width:100%;
        height: 15vh;
        background-color: #ea4a56;
        display: flex;
        justify-content: center;
        align-items: center;

        p {
            color: white;
            font-style: italic;
        }
    }
</style>