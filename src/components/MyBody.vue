<template>
    <div>
        <div class="greyArea">
            <InfoTitle :titolo="info[0].titolo" :paragrafo="info[0].paragrafo" />
        </div>
        <div class="bandAreaTitle">
            <div class="titleContainer">
                <InfoTitle :titolo="info[1].titolo" :paragrafo="info[1].paragrafo" />
            </div>
        </div>
        <div class="bandAreaCards">
            <div class="content">
                <BandNews />
            </div>
        </div>
        <PinkComponent :paragrafo="pink[0]" />
    </div>
</template>

<script>
    import InfoTitle from './InfoTitle.vue';
    import BandNews from './BandNews.vue';
    import PinkComponent from './PinkComponent.vue';


    export default {
    name: "MyBody",
    components: {
    BandNews,
    InfoTitle,
    PinkComponent
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
                ],

                pink: ['VIEW ALL LATEST NEWS', 'VIEW ALL LIVE DATES']
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
    };
    .bandAreaTitle {
        height: 30vh;
        background-color: #292d39;
        display:flex;
        flex-direction: column;
        align-items: center;
        
        
        .titleContainer {
            margin-bottom: 3rem;
            display:flex;
            justify-content:center;
            width:70%;
        }
    };
    .bandAreaCards {
        height: 170vh;
        background-color: #292d39;
        display: flex;
        justify-content: center;
    }
</style>