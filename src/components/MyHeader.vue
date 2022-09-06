<template>
    <header>
        <div class="upper-container">
            <div class="logo">
                <img src="../assets/images/avada-music-logo.png" alt="avadaLogo">
            </div>
            <div class="menu">
                <i @click="getVisible" class="fa-solid fa-bars fa-xl"></i>
            </div>
            <div :class="visible == true ? 'show-menu' : 'hide-menu'">
                <div class="myLinks">
                    <ul>
                        <li v-for="(link, index) in siteLinks" :key="index"><a href="#">{{link}}</a></li>
                    </ul>
                </div>
            </div>
        </div>
        <div :class="visible == false ? 'presentationOn' : 'presentationOff'">
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
    },
    data() {
        return {
            visible: false
        }
    },
    methods: {
        getVisible() {
            return this.visible = true;
        }
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

            .menu {
                padding-top: 1rem;
                padding-right: 2rem;
                position:relative;

                i {
                    color:white;
                    position: absolute;
                    top: 0;
                    right: 15;
                }
            };

            .hide-menu {
                display:none;

                
            }
            .show-menu {
            display:block;
            
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

                    ul {
                        list-style-type: none;
                    };

                    li {
                        margin: 3rem
                    };

                    a {
                        margin-bottom: 2rem;
                        text-decoration:none;
                        color:white;
                    }
                }
            }
        };

        .presentationOn {
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
        };
        .presentationOff {
            display:none;
        }

        

        
    }
</style>