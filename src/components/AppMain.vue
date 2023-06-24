<script>
import AppCards from'./AppCards.vue';
export default {
    AppCards
}
</script>

<template>
    <div id="jumbotron">
        <div class="container">
            <h3>CURRENT SERIES</h3>
        </div>
    </div>
    
    <div class="black-bg">
        <div class="container mid">
            <AppCards />
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/generals.scss' as *;
    @import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap');

    #jumbotron{
        background-image: url(../assets/jumbotron.jpg);
        height: 400px;
        background-size: cover;
        .container{
            position: relative;
            height: 100%;
            h3{
            background-color: #0282F9;
            color: white;
            padding: 0.4em 1.5em;
            position: absolute;
            bottom: -20px;
            font-family: 'Oswald', sans-serif;
            font-weight: 500;
            }
        }
        
    }
    .black-bg{
        background-color: #222222;
        color: white;
        padding: 2em 0;
    }

    .mid{
        display: flex;
        align-items: center;
    }
</style>