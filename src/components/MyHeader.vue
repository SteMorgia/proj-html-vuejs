<template>
    <header>
        <div class="upper-container">
            <div class="logo">
                <img src="../assets/images/avada-music-logo.png" alt="avadaLogo">
            </div>
            <div class="burgerMenu">
                <i class="fa-solid fa-bars fa-xl"></i>  
            </div>
            <div class="myLinksContainer">
                <div class="myLinks">
                    <ul>
                        <li v-for="(link, index) in siteLinks" :key="index"><a href="#">{{link}}</a></li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="presentation">
            <h1>Untold Stories</h1>
            <p>There is an untold story behind every favorite song.</p>
            <div class="buttonContainer">
                <button class="leftButton">LATEST ALBUM</button>
                <button class="rightButton">LIVE DATES</button>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'MyHeader',
    props: {
        siteLinks: Array
    }
}
</script>

<style scoped lang="scss">
    header {
        background-image: url(../assets/images/home_slider.jpg) ;
        height:100vh;
        background-size: cover;
        position:relative;
        

        .upper-container {
            display:flex;
            justify-content:space-between;
            align-items:center;
            position:relative;
            

            .logo {
                padding-top: 1rem;
                padding-left: 2rem;

                img {
                    width:80%;
                }
            };

            .burgerMenu {
                padding-top: 1rem;
                padding-right: 2rem;

                i {
                    color:white;
                }
            };

            .myLinksContainer {
                display:none;

                .myLinks {
                    width:100%;
                    height:100vh;
                    position:absolute;
                    top: 0;
                    left: 0;
                    display:flex;
                    flex-direction: column;
                    justify-content: center;
                    align-items: center;
                    background-color: #ea4a56;

                    a {
                        margin-bottom: 2rem;
                        text-decoration:none;
                        color:white;
                    }
                }
            }
        };

        .presentation {
            position: absolute;
            left:50%;
            top: 50%;
            transform: translate(-50%, -50%);
            display:flex;
            flex-direction: column;


            h1 {
                color: white;
                font-size: 90px;
                text-align: center;
            };

            p {
                color:white;
                font-size: 15px;
                text-align: center;
                font-style: italic;
                margin-top: 1rem;
            };
            .buttonContainer {
                margin-top: 2rem;
                text-align:center;

                button {
                    margin: 1rem;
                    padding: 8px 20px;
                    color: white;
                };
                .leftButton {
                    background-color: #ea4a56;
                    border: none;
                };
                .rightButton {
                    background-color: Transparent;
                    background-repeat:no-repeat;
                    border: 1px solid white;
                    cursor:pointer;
                    overflow: hidden;
                }
            }
        }

        

        
    }
</style>