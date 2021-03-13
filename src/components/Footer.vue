<template>
    <footer>
        <b-container>
             <b-row class="pb-4 text-md-left text-center">
                <b-col cols="12" md="3">
                <router-link to="/"><img alt="Company Icon" src="../assets/comp-icon.png" class="pr-3"></router-link>
                <router-link to="/"><img alt="Company Logo" src="../assets/comp-logo.png"></router-link>
                <hr class="d-none d-md-block">
                <h4  class="mt-md-0 mt-4">Australia's most trusted trades provider</h4>
                </b-col>
                <b-col cols="12" md="2" class="mt-md-0 mt-4">
                    <h5>Customers</h5>
                    <hr class="d-none d-md-block">
                    <ul class="list-unstyled">
                        <li><a href="https://getquotes.hiretrades.com.au">Get Quotes</a></li> 
                        <li><a href="/trades">200+ Trades</a></li> 
                        <li><a href="/how-it-works-customer">How it works</a></li> 
                        <li><a href="/trades-directory">Trades Directory</a></li>
                        <li><a href="/faq-customer">FAQs</a></li>
                    </ul>
                </b-col>
                <b-col cols="12" md="2" class="mt-md-0 mt-4">
                    <h5>Tradies</h5>
                    <hr class="d-none d-md-block">
                    <ul class="list-unstyled">
                        <li><router-link to="/">Register</router-link></li>
                        <li><router-link to="/">Login</router-link></li> 
                        <li><router-link to="/">How it works</router-link></li> 
                        <li><router-link to="/">FAQs</router-link></li>
                    </ul>
                </b-col>
                <b-col cols="12" md="2" class="mt-md-0 mt-4">
                    <h5>HIREtrades</h5>
                    <hr class="d-none d-md-block">
                    <ul class="list-unstyled"><li><router-link to="/">Contact Us</router-link></li> 
                        <li><router-link to="/">Our Story</router-link></li> 
                        <li><router-link to="/">Terms &amp; Conditions</router-link></li> 
                        <li><router-link to="/">Blogs</router-link></li> 
                        <li><router-link to="/">Cost Guides</router-link></li>
                    </ul>
                </b-col>
                <b-col cols="12" md="3" class="mt-md-0 mt-4">
                    <h5>Download our apps</h5>
                    <hr class="d-none d-md-block">
                    <b-row class="footer-download-apps">
                        <b-col cols="12" md="6"  class="pb-3">
                            <router-link to="/"><img alt="App Store" src="../assets/ios-black.png"></router-link>
                        </b-col>
                        <b-col cols="12" md="6" class="pb-3">
                             <router-link to="/"><img alt="Google Play" src="../assets/android-black.png"></router-link>
                        </b-col>
                    </b-row>
                    <h5 class="mt-md-0 mt-4">Follow us</h5>
                    <hr class="d-none d-md-block">
                    <ul class="footer-social list-unstyled">
                        <li><router-link to="/"><font-awesome-icon :icon="['fab', 'facebook-f']" /></router-link></li>
                        <li><router-link to="/"><font-awesome-icon :icon="['fab', 'twitter']" /></router-link></li>
                        <li><router-link to="/"><font-awesome-icon :icon="['fab', 'instagram']" /></router-link></li>
                        <li><router-link to="/"><font-awesome-icon :icon="['fab', 'pinterest']" /></router-link></li>
                        <li><router-link to="/"><font-awesome-icon :icon="['fab', 'linkedin-in']" /></router-link></li>
                    </ul>
                </b-col>
            </b-row>
            <hr class="d-none d-md-block">
              <b-row align-h="between" class="pb-3">
                <b-col cols="12" md="4">
                    <div class="copyright  text-md-left text-center">
                    <small>© 2020 - www.HIREtrades.com.au | All Rights Reserved</small>
                    </div>
                </b-col>
                <b-col cols="12" md="4">
                    <div class="privacy-policy text-md-right text-center">
                        <router-link to="/" title="Privacy Policy" class="pr-2">
                            <small>Privacy Policy</small>
                        </router-link>
                        <span class="small text-muted">|</span>
                        <router-link to="/" title="Sitemap" class="pl-2">
                            <small>Sitemap</small>
                            </router-link><span class="small text-muted">| v_2.0.78</span>
                        
                    </div>
                </b-col>
            </b-row>
        </b-container>
    </footer>
</template>

<style lang="scss">
$primary-color:#7367f0;
$secondary-color:#2c3e50;

    footer{
        background-color: #e6eaee;
        padding: 30px 0 0 0;
        a{
        color: #727e8c;
        text-decoration: none;
            &:hover{
                color: $primary-color;
                text-decoration: none;
            }
        }

        ul{
            li {
                padding: 5px 0;
            }
        }

        hr {
            border-top: 1px solid #bfbfbf!important;
            width: 25%;
            margin-left: 0;
        }
        .footer-social {
            padding: 0;
            
            li {
                display: inline-block;
                padding-right: 15px;
              
            }
            
        }
    }
</style>