<script>
import AppCards from'./AppCards.vue';
export default {
    components:{
       AppCards 
    },
    data(){
        return{
            cards: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
    
}
</script>

<template>
    <div id="jumbotron">
        <div class="container">
            <h3>CURRENT SERIES</h3>
        </div>
    </div>
    
    <div class="black-bg">
        <div class="container flex">
            <div class="row flex" >
                <div class="col" v-for="(card, index) in cards" :key="index">
                    <AppCards :image="card.thumb" :title="card.series"/>
                </div>
            </div>
            <button>LOAD MORE</button>
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
        padding: 1em 0;
        .container{
            align-items: center;
            width: 100%;
            flex-direction: column;
            .row{
                width: 100%;
                flex-wrap: wrap;
                .col{
                    width: calc(100% / 6 - 40px);
                    margin: 20px;
                }
            }
            button{
                cursor: pointer;
                background-color: #0282F9;
                color: white;
                padding: 0.5em 3em;
                font-family: 'Oswald', sans-serif;
                border: none;
                margin-top: 2em;
            }
        }
    }

</style>