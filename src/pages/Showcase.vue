<template>
    <div class="wrapper landing-page">
        <div class="page-header page-header-small rellax-header">
            <div class="page-header-image"
                 style="background-image: url('img/bg4.jpg')">
            </div>
            <div class="content-center">
                <h2 class="title">OUR WORK</h2>
                <h3>Join the snoDEV family.</h3>
                <div class="text-center">
                    <a href="https://www.linkedin.com/company/snodev" target="_blank" rel="noopener" class="btn btn-success btn-icon  btn-round">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="https://twitter.com/gosnodev" target="_blank" rel="noopener" class="btn btn-success btn-icon  btn-round">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="https://www.facebook.com/gosnodev" target="_blank" rel="noopener" class="btn btn-success btn-icon btn-round">
                        <i class="fab fa-facebook-f"></i>
                    </a>
                    <a href="https://www.instagram.com/gosnodev" target="_bank" rel="noopener" class="btn btn-success btn-icon btn-round">
                        <i class="fab fa-instagram"></i>
                    </a>
                </div>
            </div>
        </div>
        <div class="section section-examples" data-background-color="black">
            <div class="container">
                <div class="col-md-8 ml-auto mr-auto text-center">
                    <div class="section-description">
                        <h2 class="title">Not sure what you need?</h2>
                        <h5 class="description">Get some inspiration! Check out some of the components we develop. 
                        </h5>
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <h5 class="title">Services</h5>
                        <div class="card">
                            <a href="https://rlcc.netlify.com" target="_blank" rel="noopener">
                                <img v-lazy="'img/presentation-page/pages/rlccPage.png'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Contact Pages</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/snodevContactPage.png'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Logins</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/rubikonPage.png'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Signups</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/signup.jpg'" alt="">
                            </a>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <h5 class="title">Landing Pages</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/snodevLandingPage2.png'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Products</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/gatsbyLandingPage.png'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Blog Posts</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/blog-post.jpg'" alt="">
                            </a>
                        </div>
                        
                    </div>
                    <div class="col-md-4">
                        <h5 class="title">Portfolios</h5>
                        <div class="card">
                            <a href="https://tylerewald.com" target="_blank" rel="noopener">
                                <img v-lazy="'img/presentation-page/pages/tewaldPage.png'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Products</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/blkProductPage.png'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Blog Posts</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/blog-posts.jpg'" alt="">
                            </a>
                        </div>
                        <h5 class="title">Contact Pages</h5>
                        <div class="card">
                            <a>
                                <img v-lazy="'img/presentation-page/pages/blkContactPage.png'" alt="">
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
       
         
        <div class="about-contact">
            <div class="container">
                <div class="row">
                    <div class="col-md-8 mt-5 mr-auto ml-auto">
                        <h2 class="text-center title">Send us a message!</h2>
                        <h4 class="text-center description">And we'll get back to you.</h4>
                        <form class="services-form"
                            name="services"
                            action="/thankyou"
                            method="post"
                            netlify
                            netlify-honeypot="bot-field"
                        >
                            <input type="hidden" name="contact-us" value="contact-us" />
                            <div class="row">
                                <div class="col-md-4">
                                    <label>First name</label>
                                    <fg-input 
                                        name="name"
                                        addon-left-icon="now-ui-icons users_circle-08"
                                        v-model="form.firstName"
                                        placeholder="First Name...">
                                    </fg-input>
                                </div>
                                <div class="col-md-4">
                                    <label>Your email</label>
                                    <fg-input 
                                        name="email"
                                        addon-left-icon="now-ui-icons ui-1_email-85"
                                        v-model="form.email"
                                        placeholder="Email Here...">
                                    </fg-input>
                                </div>
                                <div class="col-md-4">
                                    <label>Interested Service</label>
                                    <fg-input 
                                        name="service"
                                        addon-left-icon="now-ui-icons education_atom"
                                        v-model="form.service"
                                        placeholder="How can we help?">
                                    </fg-input>
                                </div>
                            </div>
                            <div class="row">
                                <div class="col-md-4 ml-auto mr-auto text-center">
                                    <button class="btn btn-success btn-round mt-4 btn-lg">
                                        Let's talk
                                    </button>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>
<script>
  import { Card, Button, FormGroupInput, Tabs, TabPane } from '@/components';

  export default {
    name: 'showcase',
    bodyClass: 'showcase',
    components: {
      Card,
      Tabs,
      TabPane,
      [Button.name]: Button,
      [FormGroupInput.name]: FormGroupInput
    },
    head() {
        return {
            title: "%s | Showcase"
        };
    },
    data() {
      return {
        form: {
          firstName: '',
          email: '',
          message: ''
        }
      }
    }
  }
</script>
<style>
</style>