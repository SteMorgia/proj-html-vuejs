<template>
    <div class="container">
        <div class="greyArea">
            <InfoTitle :title="info[0].titolo" :paragraph="info[0].paragrafo" />
        </div>
        <BandNews />
    </div>
</template>

<script>
    import InfoTitle from './InfoTitle.vue';
    import BandNews from './BandNews.vue'


    export default {
    name: "MyBody",
    components: {
    BandNews,
    InfoTitle
},
        data() {
            return {
                info: [
                    {
                        titolo: 'Music Is Life',
                        paragrafo: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem perferendis, aliquam similique, repellendus ut sapiente!'
                    },
                    {
                        titolo: 'Latest Band News',
                        paragrafo: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem perferendis, aliquam similique, repellendus ut sapiente!'
                    },
                    {
                        titolo: 'Live Dates',
                        paragrafo: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem perferendis, aliquam similique, repellendus ut sapiente!'
                    }
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
    .greyArea {
        height: 30vh;
        background-color: #4d4d4d;
        display:flex;
        justify-content:center;
    }
</style>