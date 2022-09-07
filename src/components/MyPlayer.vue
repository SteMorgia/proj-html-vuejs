<template>
    <div class="playerContainer">
        <div class="text-container">
            <p>"I just listened to it and said to myself, "Man, I really love this album." Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're good. And they're inventive. I haven't heard anything this year that's as inventive. I don't really expect to."</p>
        </div>
        <div class="logo-container">
            <img src="../assets/images/band_interview_play_icon.png" alt="Player">
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyPlayer'
}
</script>

<style scoped lang="scss">
    .playerContainer {
        height: 80vh;
        background-image: url(../assets/images/home-testimonial-parallax.jpg);
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;

        .text-container {
            width: 50%;
            margin-bottom: 2rem;
        }

        p {
            text-align: center;
            color: white;
            font-style: italic;
            font-size: large;
        }
    }
</style>