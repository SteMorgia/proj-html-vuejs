<template>
    <div class="container">
        <h2>Latest Band News</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem perferendis, aliquam similique, repellendus ut sapiente!</p>
        <div class="cardContainer">

        </div>
    </div>  
</template>

<script>
    import SingleCardVue from './SingleCard.vue'
    export default {
        name:'BandNews',
        components: {
            SingleCard
        },
        data() {
            return {
                cards: [
                    {
                        src: "../assets/images/blog_music_techo-400x200.jpg",
                        titolo: "Technology and music",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "../assets/images/blog-post1-400x600.jpg",
                        titolo: "Taking it back to the old school",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "../assets/images/blog-post3-400x600.jpg",
                        titolo: "While my guitar gently weeps",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "../assets/images/blog-post4-400x600.jpg",
                        titolo: "It just sounds better",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "../assets/images/blog-post2-400x600.jpg",
                        titolo: "Sharing the stage with a legend",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                    {
                        src: "../assets/images/blog_flavor_rock-400x200.jpg",
                        titolo: "The flavor of rock",
                        paragrafo: "Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum."
                    },
                ]
            }
        }
    }

</script>

<style scoped lang="scss">
    .container {
        height: 200vh;
        background-color: #292d39;

        h2 {
            padding: 3rem 3rem;
            color:white;
            text-align:center;
        };
        p {
            color: white;
            text-align:center;
        }
    }
</style>