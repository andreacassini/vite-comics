<script>
export default {
    
}
</script>

<template>
    <div class="blueback">
        <div class="container">
            <ul class="flex" id="options">
                <li class="align-middle">
                    <a href="#">
                        <img src="../assets/buy-comics-digital-comics.png" alt="digital comics" style="max-width: 40px;">
                        digital comics
                    </a>
                </li>
                <li class="align-middle">
                    <a href="#">
                        <img src="../assets/buy-comics-merchandise.png" alt="dc merchandise">
                        dc merchandise
                    </a>
                </li>
                <li class="align-middle">
                    <a href="#">
                        <img src="../assets/buy-comics-subscriptions.png" alt="subscription">
                        subscription
                    </a>
                </li>
                <li class="align-middle">
                    <a href="#">
                        <img src="../assets/buy-comics-shop-locator.png" alt="comic shop locator" style="max-width: 30px;">
                        comic shop locator
                    </a>
                </li>
                <li class="align-middle">
                    <a href="#">
                        <img src="../assets/buy-dc-power-visa.svg" alt="dc power visa">
                        dc power visa
                    </a>
                </li>
            </ul>
        </div>
    </div>
    <div class="bg">
        <div class="container">
            <div class="flex">
                <ul>
                    <a href="#"><h3>DC COMICS</h3></a>
                        <a href=""><li>Characters</li></a>
                        <a href=""><li>Comics</li></a>
                        <a href=""><li>Movies</li></a>
                        <a href=""><li>Tv</li></a>
                        <a href=""><li>Games</li></a>
                        <a href=""><li>Videos</li></a>
                        <a href=""><li>News</li></a>
                </ul>
                <ul>
                    <a href=""><h3>SHOP</h3></a>
                    <a href=""><li>Shop DC</li></a>
                    <a href=""><li>Shop DC Collectibles</li></a>
                </ul>
                <ul>
                    <a href=""><h3>DC</h3></a>
                    <a href=""><li>Terms Of Use</li></a>
                    <a href=""><li>Privacy policy (New)</li></a>
                    <a href=""><li>Ad Choices</li></a>
                    <a href=""><li>Advertising</li></a>
                    <a href=""><li>Jobs</li></a>
                    <a href=""><li>Subscriptions</li></a>
                    <a href=""><li>Talent Workshops</li></a>
                    <a href=""><li>CPSC Certificates</li></a>
                    <a href=""><li>Ratings</li></a>
                    <a href=""><li>Shop Help</li></a>
                    <a href=""><li>Contact Us</li></a>
                </ul>
                <ul>
                    <a href=""><h3>SITES</h3></a>
                    <a href=""><li>DC</li></a>
                        <a href=""><li>MAD Magazine</li></a>
                        <a href=""><li>DC Kids</li></a>
                        <a href=""><li>DC Universe</li></a>
                        <a href=""><li>DC Power Visa</li></a>
                </ul>
            </div>
            <img src="../assets/dc-logo-bg.png" alt="logo">
        </div>
    </div>
    <div id="social-row">
        <div class="container flex">
            <button id="footer-btn">
                SIGN-UP NOW!
            </button>
            <div class="flex">
                <a href="#" style="margin-right: 1.2em;">FOLLOW US</a>
                <a href="#">
                    <img src="../assets/footer-facebook.png" alt="facebook">
                </a>
                <a href="#">
                    <img src="../assets/footer-twitter.png" alt="twitter">
                </a>
                <a href="#">
                    <img src="../assets/footer-youtube.png" alt="youtube">
                </a>
                <a href="#">
                    <img src="../assets/footer-pinterest.png" alt="pinterest">
                </a>
                <a href="#">
                    <img src="../assets/footer-periscope.png" alt="periscope">
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap');
    .blueback{
        background-color: #0282F9;
        padding: 2em 0;
        position: relative;
        z-index: 3;
    }

    li{
        list-style: none;
        a{
            display: flex;
            align-items: center;
            font-size: 13px;
            text-transform: uppercase;
            text-decoration: none;
            color: white;
            img{
                max-width: 50px;
                margin-right: 1em;
            }
        }
    }
    #options{
        align-items: center;
        justify-content: space-between;
    }

    .bg{
        background-image: url(../assets/footer-bg.jpg);
        height: 450px;
        background-size: cover;
        .container{
            position: relative;
            height: 100%;
            div{
                flex-direction: column;
                flex-wrap: wrap;
                height: 100%;
                align-items: flex-start;
                margin-right: 40em;
                padding: 2em 0;
                ul{
                    margin-bottom: 1.5em;
                    a{
                        text-decoration: none;
                        h3{
                        font-size: 20px;
                        font-family: 'Oswald', sans-serif;
                        margin-bottom: 0.8em;
                        color: white;
                        }
                        li{
                            color: grey;
                            line-height: 1.5;
                        }
                    }   
                }
            }  
            img{
                position: absolute;
                right: 0;
                top: -120px;
                width: 58%;
            }
        }
    }

    #footer-btn{
        border-color: #0282F9;
        background-color: transparent;
        color: white;
        font-weight: bold;
        padding: 1em;
        cursor: pointer;
    }
    #social-row{
        background-color: #303030;
        padding: 2em 0;
        position: relative;
        z-index: 2;
        
        .container{
            align-items: center;
            justify-content: space-between;
            div{
                align-items: center;
                a{
                    color: #0282F9;
                    font-weight: bold;
                    text-decoration: none;
                    font-family: 'Oswald', sans-serif;
                    margin: 0 0.4em;
                }
                
            }
        }
    }
</style>