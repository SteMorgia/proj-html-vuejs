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
        <MyPlayer />
        <div class="datesArea">
            <InfoTitle :titolo="info[2].titolo" :paragrafo="info[2].paragrafo" />
            <div class="datesPlaces">
                <MyDates :dates="dates"/>
            </div>
        </div>
        <PinkComponent :paragrafo="pink[1]" />
    </div>
</template>

<script>
    import InfoTitle from './InfoTitle.vue';
    import BandNews from './BandNews.vue';
    import PinkComponent from './PinkComponent.vue';
    import MyPlayer from './MyPlayer.vue';
    import MyDates from './MyDates.vue'


    export default {
    name: "MyBody",
    components: {
    BandNews,
    InfoTitle,
    PinkComponent,
    MyPlayer,
    MyDates,
    
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

                pink: ['VIEW ALL LATEST NEWS', 'VIEW ALL LIVE DATES'],

                dates: ['17/08/2022 GEM FESTIVAL 2022 ANAKALIA, GEORGIA', '24/9/2022 GROOVEFEST DOMINICAL REPUBLIC', '31/10/2022 OASIS FESTIVAL 2022 MARRAKECH, MOROCCO', '07/11/2022 MOGA FESTIVAL - ESSAOURIA, MOROCCO', '10/12/2022 ENVISION FESTIVAL - UVITA, COSTA RICA']
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
        max-height: 170vh;
        background-color: #292d39;
        display: flex;
        justify-content: center;
        padding-bottom: 3rem;
    };
    .datesArea {
        max-height: 200vh;
        background-color: #292d39;
        display: flex;
        flex-direction: column;
        align-items:center;

        .datesPlaces {
            margin: 2rem;
            
        }
    }
</style>