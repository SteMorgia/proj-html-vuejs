<template>
    <header>
        <div class="upper-container">
            <div class="logo">
                <img src="../assets/images/avada-music-logo.png" alt="avadaLogo">
            </div>
            <div class="burgerMenu">
                <i class="fa-solid fa-bars fa-xl"></i>  
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'MyHeader'
}
</script>

<style scoped lang="scss">
    header {
        background-image: url(../assets/images/home_slider.jpg) ;
        height:100vh;
        background-size: cover;

        .upper-container {
            display:flex;
            justify-content:space-between;
            align-items:center;

            .logo {
                padding-top: 1rem;
                padding-left: 2rem;

                img {
                    width:80%;
                }
            }
        };

        .burgerMenu {
            padding-top: 1rem;
            padding-right: 2rem;

            i {
                color:white;
            }
        }
    }
</style>