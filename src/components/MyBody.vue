<template>
    <div class="container">
        <MyBodyIntro />
        <BandNews />
    </div>
</template>

<script>
    import MyBodyIntro from './MyBodyIntro.vue';
    import BandNews from './BandNews.vue'

export default {
    name: "MyBody",
    components: { 
        MyBodyIntro,
        BandNews
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

</style>