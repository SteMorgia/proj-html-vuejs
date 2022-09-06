<template>
    <div class="container">
        <div class="cardContainer">
            <SingleCard v-for="(card, index) in cards" :key="index" :imageSrc="card.src" :titolo="card.titolo" :paragrafo="card.paragrafo" />
        </div>
    </div>  
</template>

<script>
    
    import SingleCard from './SingleCard.vue'
    export default {
        name:'BandNews',
        components: {
            SingleCard,
            
        },
        data() {
            return {
                cards: [
                    {
                        src: "images/blog_music_techo-400x200.jpg",
                        titolo: "Technology and music",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
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
                    {
                        src: "images/blog_flavor_rock-400x200.jpg",
                        titolo: "The flavor of rock",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                ]
            }
        }
    }

</script>

<style scoped lang="scss">
    .cardContainer {
        display: flex;
        flex-wrap: wrap;
        width: 60%;
    }
    
</style>