<template>
    <div class="footerContainer">
        <div class="logoContainer">
            <img src="../assets/images/avada-music-logo.png" alt="Logo">
        </div>
        <div class="linksContainer">
            <ul>
                <li v-for="(link, index) in siteLinks" :key="index"><a href="#">{{link}}</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyFooter',
    props: {
        siteLinks: Array
    }
}
</script>

<style scoped lang="scss">
    .footerContainer {
        height: 20vh;
        background-color: #292d39;
        display:flex;
        justify-content: space-between;
        align-items: center;

        .logoContainer {
            padding: 1rem;
        };
        .linksContainer {
            padding: 1rem;

            ul {
                list-style-type: none;
                

                li {
                    display: inline-block;
                    margin: 5px;
                    

                    a {
                        color: white;
                        text-decoration: none;
                        font-size: 13px;
                    }
                }
            }
        }
    }
</style>