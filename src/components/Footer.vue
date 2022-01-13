<template>
    <footer>
        <div class="upper-footer">
            <div class="container">
                <div class="col-1">
                    <div class="col-1a">
                        <h3 class="footer-title">Dc Comics</h3>
                        <ul>
                            <li> <a href="#"> Characters </a></li>
                            <li> <a href="#"> Comics </a></li>
                            <li> <a href="#"> Movies </a></li>
                            <li> <a href="#"> Tv </a></li>
                            <li> <a href="#"> Games </a></li>
                            <li> <a href="#"> Videos </a></li>
                            <li> <a href="#"> News </a></li>
                        </ul>
                        <h3 class="footer-title">Shop</h3>
                        <ul>
                            <li> <a href="#"> Shop DC </a></li>
                            <li> <a href="#"> Shop DC Collectibles </a></li>

                        </ul>
                    </div>
                    <div class="col-1b">
                        <h3 class="footer-title">Dc</h3>
                        <ul>
                            <li> <a href="#"> Terms Of Use </a></li>
                            <li> <a href="#"> Privacy policy (New) </a></li>
                            <li> <a href="#"> Ad Choices </a></li>
                            <li> <a href="#"> Advertising </a></li>
                            <li> <a href="#"> Jobs </a></li>
                            <li> <a href="#"> Subscriptions </a></li>
                            <li> <a href="#"> Talent Workshops </a></li>
                            <li> <a href="#"> CPSC Certificates </a></li>
                            <li> <a href="#"> Ratings </a></li>
                            <li> <a href="#"> Shop Help </a></li>
                            <li> <a href="#"> Contact Us </a></li>
                            
                        </ul>
                    </div>
                    <div class="col-1c">
                        <h3 class="footer-title">Sites</h3>
                        <ul>
                            <li> <a href="#"> DC </a></li>
                            <li> <a href="#"> MAD Magazine </a></li>
                            <li> <a href="#"> DC Kids </a></li>
                            <li> <a href="#"> DC Universe </a></li>
                            <li> <a href="#"> DC Power Visa </a></li>
                            
                        </ul>
                    </div>
                </div>
                <div class="col-2">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>

        <div class="lower-footer">
            <div class="container">
                <div class="col-lower">
                    <a href="#" class="sign-me"> Sign-Up Now! </a>
                </div>
                <div class="col-lower-b">
                    <h2> Follow Us </h2>
                    <ul>
                        <li> <a href="#"></a> <img src="../assets/img/footer-facebook.png" alt=""> </li>
                        <li> <a href="#"> <img src="../assets/img/footer-twitter.png" alt=""> </a> </li>
                        <li> <a href="#"> <img src="../assets/img/footer-youtube.png" alt=""> </a> </li>
                        <li> <a href="#"> <img src="../assets/img/footer-pinterest.png" alt=""> </a> </li>
                        <li> <a href="#"> <img src="../assets/img/footer-periscope.png" alt=""> </a> </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style lang="scss">

    footer {

        display: flex;
        flex-direction: column;

        .upper-footer {

            background-image: url('../assets/img/footer-bg.jpg');
            background-size: cover;
            width: 100%;
            height: 400px;

            .container {

                display: flex;
                justify-content: space-between;
                align-items: center;
                height: 400px;

                .col-1 {

                    display: flex;
                    justify-content: space-around;
                    width: 40%;

                }
                .col-2 {
                    width: 60%;
                    display: flex;
                    justify-content: flex-end;

                    img {
                        width: 60%;
                    }
                }
            }

            h3 {
                text-transform: uppercase;
                color: #FFFFFF;
                margin-top: 1em;
                margin-bottom: 0.6em;
            }

            ul {

                list-style-type: none;
                
                li {
                    list-style-type: none;
                    margin-bottom: 0.2em;
                    a {
                        color: #959595;
                        text-decoration: none;
                    }
                }
            }
            
        }

        .lower-footer {

            background-color: #303030;
            width: 100%;
            height: 104px;

            .container {
                display: flex;

                .col-lower {
                    width: 70%;
                    height: 104px;
                    display: flex;
                    align-items: center;

                    a {
                        text-transform: uppercase;
                        color: #FFFFFF;
                        font-weight: bold;
                        display: block;
                        text-decoration: none;
                        padding: 0.8em;
                        border: 3px solid #0282F9;
                        margin-left: 1.2em;
                    
                    }
                }
                .col-lower-b {
                    width: 30%;
                    height: 104px;
                    display: flex;
                    align-items: center;

                    h2 {
                        color: #0282F9;
                        text-transform: uppercase;
                        font-size: 1.3em;
                    }

                    ul {
                        list-style-type: none;
                        display: flex;
                        width: 70%;
                        justify-content: space-around;
                        
                        li {
                            list-style-type: none;
                            margin-bottom: 0.2em;
                            display: block;

                            a {
                                color: #959595;
                                text-decoration: none;
                            }
                        }
                    }
                }
            }
        }
    }
</style>