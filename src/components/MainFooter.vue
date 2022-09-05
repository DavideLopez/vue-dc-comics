<template>
    <footer>
        <div class="features">
            <ul class="container feature-list">
                <li class="feature-item">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                    Digital comics
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-comics-merchandise.png" alt="">
                    DC merchandise
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-comics-subscriptions.png" alt="">
                    Subscription
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-comics-shop-locator.png" alt="">
                    Comic shop locator
                </li>
                <li class="feature-item">
                    <img src="../assets/buy-dc-power-visa.svg" alt="">
                    DC power visa
                </li>
            </ul>
        </div>
        <div class="nav">
            <div class="container">
                <div>
                    <h3 class="footer-explore">DC comics</h3>
                    <ul>
                        <li><a class="links" href="#">Characters</a></li>
                        <li><a class="links" href="#">Comics</a></li>
                        <li><a class="links" href="#">Movies</a></li>
                        <li><a class="links" href="#">TV</a></li>
                        <li><a class="links" href="#">Games</a></li>
                        <li><a class="links" href="#">Videos</a></li>
                        <li><a class="links" href="#">News</a></li>
                    </ul>
                    <h3 class="footer-explore">Shop</h3>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="footer-explore">DC</h3>
                    <ul>
                        <li><a href="#">Terms of use</a></li>
                        <li><a href="#">Privacy Policy (new)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="footer-explore">Sites</h3>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>
        <div class="footer-cta">
            <div class="container">
                <a class="button" href="#">Sign-up now!</a>
                <div class="socials">
                    <h3>Follow us</h3>
                    <ul class="social-list">
                        <li><a class="socialbutton" href="#"><img src="../assets/footer-facebook.png" alt=""></a></li>
                        <li><a class="socialbutton" href="#"><img src="../assets/footer-twitter.png" alt=""></a></li>
                        <li><a class="socialbutton" href="#"><img src="../assets/footer-youtube.png" alt=""></a></li>
                        <li><a class="socialbutton" href="#"><img src="../assets/footer-pinterest.png" alt=""></a></li>
                        <li><a class="socialbutton" href="#"><img src="../assets/footer-periscope.png" alt=""></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>

    
</template>


<script>
    export default {

    }
</script>

<style lang="scss" scoped>
    .features {
        padding: 3rem 0;
        background-color: #0282f9;

        .feature-list {
            display: flex;
            flex-wrap: wrap;
        }

        .feature-item {
            flex-basis: 0;
            flex-grow: 1;

            display: flex;
            justify-content: center;
            align-items: center;
            gap: 12px;
            color: #fff;
            text-transform: uppercase;

            img {
                width: 60px;
                aspect-ratio: 1 / 1;
                object-fit: contain;
            }
        }
    }

    .nav {
        padding: 3rem 0;
        background: url('../assets/footer-bg.jpg') center/cover no-repeat #1c1c1c;
        color: #fff;
        overflow: hidden;

        .container {
            display: flex;
            gap: 1.5em;
            position: relative;

            img {
                width: 560px;
                margin-left: auto;
                position: absolute;
                top: 50%;
                right: 0;
                transform: translateY(-50%);
            }

            a {
                color: gray;
                font-size: 12px;
            }

            a:hover {
                color: white;
            }

            .footer-explore {
                padding-top: 15px;
                padding-bottom: 15px;
            }

        
        }
    }

    .footer-cta {
        padding: 1.5rem 0;
        background-color: #303030;
        color: #fff;

        .container {
            display: flex;
            align-items: center;
            gap: 1rem;

            .button {
                display: block;
                padding: 8px 12px;
                border: 2px solid #0282f9;
                margin-right: auto;
                text-transform: uppercase;
            }

            .button:hover {
                opacity: 0.5;
            }
            
            .socials {
                display: contents;

                h3 {
                    color: #0282f9;
                    text-transform: uppercase;
                }

                .social-list {
                    display: flex;
                    gap: 1rem;
                }

                .socialbutton:hover {
                    opacity: 0.5;
                }
            }
        }
    }

</style>