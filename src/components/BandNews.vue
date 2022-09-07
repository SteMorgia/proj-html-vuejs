<template>
    <div class="container">
        <div class="cardContainerLeft">
            <SingleCardOrizzontale :imageSrc="cardsOrizzontali[0].src" :titolo="cardsOrizzontali[0].titolo" :paragrafo="cardsOrizzontali[0].paragrafo" />
            <SingleCardVerticale :imageSrc="cardsVerticali[1].src" :titolo="cardsVerticali[1].titolo" :paragrafo="cardsVerticali[1].paragrafo" />
            <SingleCardVerticale :imageSrc="cardsVerticali[2].src" :titolo="cardsVerticali[2].titolo" :paragrafo="cardsVerticali[2].paragrafo" />
            <SingleCardOrizzontale :imageSrc="cardsOrizzontali[1].src" :titolo="cardsOrizzontali[1].titolo" :paragrafo="cardsOrizzontali[1].paragrafo" />

        </div>
        <div class="containerRight">
            <SingleCardVerticale :imageSrc="cardsVerticali[0].src" :titolo="cardsVerticali[0].titolo" :paragrafo="cardsVerticali[0].paragrafo" />
            <SingleCardVerticale :imageSrc="cardsVerticali[3].src" :titolo="cardsVerticali[3].titolo" :paragrafo="cardsVerticali[3].paragrafo" />

        </div>
    </div>  
</template>

<script>
    import SingleCardVerticale from './SingleCardVerticale.vue';
    import SingleCardOrizzontale from './SingleCardOrizzontale.vue'
    export default {
        name:'BandNews',
        components: {
            SingleCardOrizzontale,
            SingleCardVerticale
        },
        data() {
            return {
                cardsOrizzontali: [
                    {
                        src: "images/blog_music_techo-400x200.jpg",
                        titolo: "Technology and music",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    
                    {
                        src: "images/blog_flavor_rock-400x200.jpg",
                        titolo: "The flavor of rock",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                ],
                cardsVerticali: [
                    {
                        src: "images/blog-post1-200x300.jpg",
                        titolo: "Taking it back to the old school",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "images/blog-post3-200x300.jpg",
                        titolo: "While my guitar gently weeps",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "images/blog-post4-200x300.jpg",
                        titolo: "It just sounds better",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "images/blog-post2-200x300.jpg",
                        titolo: "Sharing the stage with a legend",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                ]
            }
        }
    }

</script>

<style scoped lang="scss">
.container {
    width: 100%;
    display: flex;
}

    .cardContainerLeft {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        width: 450px;
        
    };
    .cardContainerRight {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        width: 230px;
        
    }
    
</style>