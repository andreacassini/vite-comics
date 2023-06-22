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
    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        
    }
    li{
        display: inline;
        padding: 3.5em 0.8em;
        a{
            text-decoration: none;
            color: black;
            font-size: 14px;
        }
    }
</style>