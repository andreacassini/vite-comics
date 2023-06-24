<script>
export default {
    data() {
        
        return {
            menu : [
                {
                    'cat' : 'CHARACTERS',
                    'active' : false
                },
                {
                    'cat' : 'COMICS',
                    'active' : true
                },
                {
                    'cat' : 'MOVIES',
                    'active' : false
                },
                {
                    'cat' : 'TV',
                    'active' : false
                },
                {
                    'cat' : 'GAMES',
                    'active' : false
                },
                {
                    'cat' : 'COLLECTIBLES',
                    'active' : false
                },
                {
                    'cat' : 'VIDEOS',
                    'active' : false
                },
                {
                    'cat' : 'FANS',
                    'active' : false
                },
                {
                    'cat' : 'NEWS',
                    'active' : false
                },
                {
                    'cat' : 'SHOP',
                    'active' : false
                },
            ]
          }
      }
}
</script>

<template>
    <div class="container">    
        <img src="../assets/dc-logo.png" alt="logo">
        <ul>
            <li v-for="(cat, index) in menu" :key="index">
                <a href="#">
                    {{ cat.cat }}
                </a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
    @use '../styles/generals.scss' as *;
    @import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap');
    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1em;
    }
    li{
        display: inline;
        padding: 3.6em 0.8em;
        a{
            text-decoration: none;
            font-size: 14px;
            font-weight: bold;
            font-family: 'Oswald', sans-serif;
            color: rgb(71, 71, 71);
        }
    }
</style>