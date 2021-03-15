<template>
  <div class="home">
   
      <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
      <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
      <div id="what-we-do">
         <b-container>
        <h2 class="title">How HIREtrades works</h2>
        <b-row class="my-5">
          <b-col cols="12" md="4">
            <div class="what-we-do-details">
              <b-row>
                    <b-col cols="3">
                      <div class="what-we-do-details-number">
                        1
                      </div>
                    </b-col>
                    <b-col cols="9">
                      <div class="what-we-do-details-description">
                        <h3>Post a job</h3>
                        <p>It takes 2 minutes</p>
                      </div>
                    </b-col>
              </b-row>
            </div>
          </b-col>
          <b-col cols="12" md="4">
            <div class="what-we-do-details">
              <b-row>
                <b-col cols="3">
                      <div class="what-we-do-details-number">
                        2
                      </div>
                    </b-col>
                    <b-col cols="9">
                      <div class="what-we-do-details-description">
                        <h3>Get quotes</h3>
                        <p>Tradies get in touch</p>
                      </div>
                    </b-col>
                </b-row>
              </div>
            </b-col>
          <b-col cols="12" md="4">
            <div class="what-we-do-details">
              <b-row>
                    <b-col cols="3">
                      <div class="what-we-do-details-number">
                        3
                      </div>
                    </b-col>
                    <b-col cols="9">
                      <div class="what-we-do-details-description">
                        <h3>Rate and review</h3>
                        <p>Job complete. Leave feedback</p>
                      </div>
                    </b-col>
              </b-row>
            </div>
          </b-col>
        </b-row>
         </b-container>
      </div>
   
    
      <!-- what-we-do end section-->
      <div id="inspirational-panel">
        <b-container>
          <h2 class="title text-center mb-4">Inspirational Panel</h2>
          <b-row class="align-items-stretch">
            <b-col cols="12" md="8">
              <!-- <div> -->
              <b-card no-body class="overflow-hidden align-self-start">
                <b-row no-gutters>
                  <b-col cols="5" >
                    <div class="d-block inspirational-panel-img" v-bind:style="{ backgroundImage: 'url(' + cost_guides_image + ')' }">
                    </div>
                  </b-col>
                  <b-col cols="7">
                    <b-card-body class="p-4" title="Cost Guides">
                      <b-card-text class="mb-3">
                        Research to assist consumers with Trades pricing.
                        
                      </b-card-text>
                      <div>
                        <router-link to="/" class="mb-2 d-block">View prices</router-link>
                        </div>
                    </b-card-body>
                  </b-col>
                </b-row>
              </b-card>
            <!-- </div> -->
              <!-- <div> -->
              <b-card no-body class="overflow-hidden align-self-end">
                <b-row no-gutters>
                  <b-col cols="7">
                    <b-card-body class="p-4" title="Blogs">
                      <b-card-text class="mb-3">
                        Articles of interest and great ideas.
                        
                      </b-card-text><br>
                      <div>
                        <router-link to="/" class="mb-2 d-block">Discover more</router-link>
                        </div>
                    </b-card-body>
                  </b-col>
                  <b-col cols="5">
                    <div class="d-block inspirational-panel-img" v-bind:style="{ backgroundImage: 'url(' + cost_blog_image + ')' }">
                    </div>
                    <!-- <b-card-img src="https://picsum.photos/400/400/?image=20" alt="Image" class="rounded-0"  img-right></b-card-img> -->
                  </b-col>
                </b-row>
              </b-card>
            <!-- </div> -->
            </b-col>
            <b-col cols="12" md="4">
              <!-- <div> -->
              <b-card no-body class="overflow-hidden align-self-start">
                <b-row no-gutters>
                  <b-col cols="5" md="12">
                    <div class="d-block inspirational-panel-img ask-tradie" v-bind:style="{ backgroundImage: 'url(' + cost_ask_tridie_image + ')' }">
                    </div>
                  </b-col>
                  <!-- <b-col sm="12">
                    <div class="d-block inspirational-panel-img ask-tradie" v-bind:style="{ backgroundImage: 'url(' + cost_guides_image + ')' }">
                    </div>
                  </b-col> -->
                  <b-col cols="7" md="12">
                    <b-card-body class="p-4" title="Ask a Tradie">
                      <b-card-text class="mb-3">
                        Our network of Tradies can help answer your questions.
                      </b-card-text>
                      <div>
                        <router-link to="/" class="mb-2 d-block">What's your question?</router-link>
                        </div>
                    </b-card-body>
                  </b-col>
                </b-row>
              </b-card>
            <!-- </div> -->
            </b-col>
          </b-row>    
         </b-container>  
      </div>
      <!-- inspirational-panel end section-->
    
    
      <div id="testimonials">
        <b-container>
          <h2 class="title">What homeowners are saying</h2>
          <b-row class="no-gutters">
              <b-col cols="12" md="4" class="text-center mb-lg-0 mb-4">
                <b-card class="shadow">
                  <b-img :src="require('../assets/jodie.webp')"  rounded="circle"  v-bind="testimonialProfile" class="mb-4"></b-img>
                  <b-card-text><i>
                    "You make life really easy for last minute people like me. 
                    I'm always time challenged and not wanting to spend the time chasing Tradies. 
                    Two minutes to post a job. Right price, right quality, right timing. 
                    No stress whatsoever. Thanks HIREtrades."</i>
                  </b-card-text>
                  <b-card-text class="name">
                    <b>Jodie, NSW</b>
                  </b-card-text>
                </b-card>
              </b-col>
               <b-col cols="12" md="4" class=" text-center  mb-lg-0 mb-4">
                <b-card class="shadow">
                  <b-img :src="require('../assets/kenvacation.webp')"  rounded="circle"  v-bind="testimonialProfile" class="mb-4"></b-img>
                  <b-card-text><i>
                    "You make life really easy for last minute people like me. 
                    I'm always time challenged and not wanting to spend the time chasing Tradies. 
                    Two minutes to post a job. Right price, right quality, right timing. 
                    No stress whatsoever. Thanks HIREtrades."</i>
                  </b-card-text>
                  <b-card-text class="name">
                    <b>Jodie, NSW</b>
                  </b-card-text>
                </b-card>
              </b-col>
               <b-col cols="12" md="4" class="text-center mb-lg-0 mb-4">
                <b-card class="shadow">
                  <b-img :src="require('../assets/joseph-sydney.webp')"  rounded="circle"  v-bind="testimonialProfile" class="mb-4"></b-img>
                  <b-card-text><i>
                    "You make life really easy for last minute people like me. 
                    I'm always time challenged and not wanting to spend the time chasing Tradies. 
                    Two minutes to post a job. Right price, right quality, right timing. 
                    No stress whatsoever. Thanks HIREtrades."</i>
                  </b-card-text>
                  <b-card-text class="name">
                    <b>Jodie, NSW</b>
                  </b-card-text>
                </b-card>
              </b-col>
          </b-row>
        </b-container>
      </div>

      <div id="download-app">
        <b-container>
         <b-row class="no-gutters">
          <b-col cols="12" md="6">
            <div class="download-app-details text-md-left text-center">
              <h3 class="pb-4">Download the HIREtrades App</h3>
              <ul class="list-unstyled">
                <li><font-awesome-icon icon="tag" />Stay updated</li>
                <li><font-awesome-icon icon="tag" />Chat on the go</li>
                <li><font-awesome-icon icon="tag" />Request anytime</li>
                <li><font-awesome-icon icon="tag" />Attach files directly</li>
              </ul>
              <b-row class="download-app-image mt-5">
                <b-col lg="5" class="mb-lg-0 mb-4">
                  <router-link to="/"><img alt="App Store" src="../assets/ios-app-download.webp" class="img-fluid"></router-link>
                </b-col>
                <b-col lg="5">
                  <router-link to="/"> <img alt="Google Play" src="../assets/android-app-download.webp" class="img-fluid"></router-link>
                </b-col>
              </b-row>
            </div>

          </b-col>
          <b-col cols="12" md="6">
              <div class="app-img text-center d-none d-md-block">
               <img alt="Mobile" src="../assets/mockup-iphone-thin.webp">
               </div>
          </b-col>
        </b-row>
        </b-container>
      </div>

      <div id="top-trades">
        <b-container>
        <h2 class="title">Our Top Trades</h2>
        <b-row class="mt-5">
          <b-col class="text-center">
            <h3>Sydney</h3>
            <ul class="list-unstyled">
              <li><router-link to="/">Painters</router-link></li>
              <li><router-link to="/">Pest Control</router-link></li>
              <li><router-link to="/">Electricians</router-link></li>
              <li><router-link to="/">Plumbers</router-link></li>
              <li><router-link to="/">Concreting</router-link></li>
              <li><router-link to="/">Carpenters</router-link></li>
            </ul>
          </b-col>
          <b-col class="text-center">
            <h3>Melbourne</h3>
            <ul class="list-unstyled">
              <li><router-link to="/">Handyman</router-link></li>
              <li><router-link to="/">Electricians</router-link></li>
              <li><router-link to="/">Concreting</router-link></li>
              <li><router-link to="/">Painters</router-link></li>
              <li><router-link to="/">Plumbers</router-link></li>
              <li><router-link to="/">Bricklaying</router-link></li>
            </ul>
          </b-col>
          <b-col class="text-center">
            <h3>Brisbane</h3>
            <ul class="list-unstyled">
              <li><router-link to="/">Pest Control</router-link></li>
              <li><router-link to="/">Painters</router-link></li>
              <li><router-link to="/">Fencing</router-link></li>
              <li><router-link to="/">Handyman</router-link></li>
              <li><router-link to="/">Electricians</router-link></li>
              <li><router-link to="/">Air Conditioning</router-link></li>
            </ul>
          </b-col>
          <b-col class="text-center">
            <h3>Perth</h3>
            <ul class="list-unstyled">
              <li><router-link to="/">Plumbers</router-link></li>
              <li><router-link to="/">Painters</router-link></li>
              <li><router-link to="/">Carpenters</router-link></li>
              <li><router-link to="/">Electricians</router-link></li>
              <li><router-link to="/">Air Conditioning</router-link></li>
              <li><router-link to="/">Kitchen</router-link></li>
            </ul>
          </b-col>
          <b-col class="text-center">
            <h3>Adelaide</h3>
            <ul class="list-unstyled">
              <li><router-link to="/">Painters</router-link></li>
              <li><router-link to="/">Fencing</router-link></li>
              <li><router-link to="/">Builder</router-link></li>
              <li><router-link to="/">Electricians</router-link></li>
              <li><router-link to="/">Handyman</router-link></li>
              <li><router-link to="/">Air Conditioning</router-link></li>
            </ul>
          </b-col>
          
        </b-row>
        </b-container>
      </div>
    
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import cost_guides_image from "@/assets/accounting-balance-banking.webp"
import cost_blog_image from "@/assets/organise.webp"
import cost_ask_tridie_image from "@/assets/blueprint-designing-diagram.webp"

export default {
  name: 'Home',
  components: {
    // HelloWorld
  },
  
  data() {
    return {
      inspirational_panel: {
        // width: '100%',
        // height: '100%',
        //'background-image': 'url(../assets/accounting-balance-banking.webp)',
      },
      cost_guides_image,
      cost_blog_image,
      cost_ask_tridie_image,
      testimonialProfile: { blank: false, blankColor: '#777', width: 75, height: 75, class: 'm1' }
    };
    
  },
}
</script>


<style lang="scss">
$primary-color:#475f7b;
$secondary-color:#2c3e50;
$third-color:#727e8c;
$lavender-color:#7367f0;

body{
    font-family: "IBM Plex Sans",Helvetica,Arial,serif;
    color: $primary-color!important;
    font-size: 16px;
    font-weight: 400;
    p{
      line-height: 2rem;
      color: #666;
    }
}

a{
  color: $third-color !important;
  font-size: 16px;
  text-decoration: none;
    &:hover{
        color: $lavender-color !important;
        text-decoration: none !important;
    }
}

h2{
  color:$primary-color;
  &.title{
    text-align: center;
    &:after{
      content: url('../assets/divider.png');
      display: block;
    }
  }
}

h3{
  color:$primary-color;
}
 
#what-we-do{
  padding: 80px 0;
}

.navbar-nav{
  li{
    a {
      padding: 20px 15px;
    }
  }
}

.what-we-do-details{
  &-number {
    font-size: 60px;
    color: $lavender-color;
    position: relative;
    top: -13px;
    font-weight: 300;
    text-align: center;
  }
  &-description {
    text-align: left;
  }
}

#inspirational-panel{
      // text-align: left;
    h4{
      font-size: 1.73rem;
    }
    .card{
      box-shadow: -8px 12px 18px 0 rgb(25 42 70 / 13%);
      margin-bottom: 2.2em;
      border: none;
      border-radius: 0;
    }
  .inspirational-panel-img{
    height: 100%;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  a{
    color: $lavender-color !important;
    &:hover{
      text-decoration: underline !important;
    }
  }

  .ask-tradie{
    min-height: 202px;
  }
}
#testimonials{
  padding: 220px 0 180px 0;
  background-color: #fff;
  .card {
    border: 0px !important;
    padding: 20px;
  }
}

#download-app{
  padding: 70px 0;
  background-color: #E7EBED;
  .download-app-details{
  h3{
    font-size: 2.53rem;
  }
  li {
    font-size: 1.47rem;
    color:$primary-color;
    padding: 8px 0;
      svg {
        font-size: 15px;
        color: #828D99;
        position: relative;
        top: -3px;
        margin-right:10px ;
      }
    }
  }
  .app-img img {
      margin: auto;
      position: absolute;
      top: 0;
      left: 0;
      bottom: 0;
      right: 0;
  }
}


#top-trades {
  padding: 80px 0;
  ul{
    li{
      padding: 5px 0;
    }
  }
}
</style>