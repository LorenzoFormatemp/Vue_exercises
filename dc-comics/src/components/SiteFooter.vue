<script>

import icons from '../assets/data/social.js'

export default {
    name: 'SiteFooter',
    data() {
        return {
            icons: icons
        }
    }
}
</script>

<template>

    <footer id="site_footer">

        <!-- top -->
        <div class="footer-top">
            <div class="container">
                
                <!-- Categorie -->
                <div class="col">
                    <h3>Dc Comics</h3>

                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">Tv</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>

                    <div class="shop">
                        <h3>Shop</h3>
                        <ul>
                            <li>
                                <a href="#">Shop Dc</a>
                            </li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>


                </div>
                
                <!-- Termini e condizioni -->
                <div class="col">
                    <h3>DC</h3>

                    <ul>
                        <li>
                            <a href="#">Terms of use</a>
                        </li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                    </ul>

                </div>


                <div class="col">
                    <h3>Sites</h3>
                    <ul>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                        <li><a href="#">text</a></li>
                    </ul>
                </div>
            </div>


        </div>

        <!-- bottom -->
        <div class="footer-bottom">

            <div class="container">
                <div class="col">
                    <div class="btn">
                        <a>Sign UP Now!</a>
                    </div>
                </div>

                <div class="social">
                    <div class="follow">Follow Us</div>
                    <img :src="icon.path" alt="social-icon-img" v-for="icon in icons">

                </div>


            </div>

        </div>
    </footer>


</template>