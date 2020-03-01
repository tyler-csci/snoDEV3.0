<template>
    <div class="wrapper landing-page">
        <div class="page-header page-header-small rellax-header">
            <div class="page-header-image"
                 style="background-image: url('img/bg4.jpg')">
            </div>
            <div class="content-center">
                <h2 class="title">SERVICES</h2>
                <h3>IT'S 2020. YOUR WEBSITE SHOULD LOOK LIKE IT.</h3>
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

        <div class="separator-line separator-primary"></div>
            <div class="container">
                <div class="row">
                    <div class="col-md-8 ml-auto mt-5 mr-auto">
                        <h2 class="title text-center">Popular Services</h2>
                        <h4 class="description text-center">Aside from building websites, these are other popular services we offer. 
                                If you need something but don't see it, send us a message!</h4>
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <div class="info info-hover">
                            <div class="icon icon-info">
                                <i class="now-ui-icons ui-2_chat-round"></i>
                            </div>
                            <h4 class="info-title">Free Consultation</h4>
                            <p class="description">Tell us about your project and we'll give you an honest, in-depth solution.</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="info info-hover">
                            <div class="icon icon-info">
                                <i class="now-ui-icons business_chart-pie-36"></i>
                            </div>
                            <h4 class="info-title">Performance Testing</h4>
                            <p class="description">See how well your website performs and how it can be improved.</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="info info-hover">
                            <div class="icon icon-info">
                                <i class="now-ui-icons design-2_ruler-pencil"></i>
                            </div>
                            <h4 class="info-title">Data Analytics</h4>
                            <p class="description">Track users, sessions, pageviews, etc. See user behavior and how to increase conversions.</p>
                        </div>
                    </div>
                </div>
                <div class="row">
                    <div class="col-md-4">
                        <div class="info info-hover">
                            <div class="icon icon-info">
                                <i class="now-ui-icons ui-2_chat-round"></i>
                            </div>
                            <h4 class="info-title">SEO Optimization</h4>
                            <p class="description">See how your website is currently optimized and how it can climb the ranks of search engines.</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="info info-hover">
                            <div class="icon icon-info">
                                <i class="now-ui-icons business_chart-pie-36"></i>
                            </div>
                            <h4 class="info-title">CMS</h4>
                            <p class="description">Integrate an easy-to-use content management system to your website. CMS is great for blogs and news.</p>
                        </div>
                    </div>
                    <div class="col-md-4">
                        <div class="info info-hover">
                            <div class="icon icon-info">
                                <i class="now-ui-icons design-2_ruler-pencil"></i>
                            </div>
                            <h4 class="info-title">Third Party Integrations</h4>
                            <p class="description">Need a specific plugin or API but not sure how to add it to your site? We can do it for you!</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="separator-line separator-primary"></div>


        

        

            
        <div class="about-contact">
            <div class="container">
                <div class="row">
                    <div class="col-md-8 mt-5 mr-auto ml-auto">
                        <h2 class="text-center title">Want to know more about a specific service?</h2>
                        <h4 class="text-center description">Send us your info and we'll get back to you!</h4>
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
    name: 'services',
    bodyClass: 'services',
    components: {
      Card,
      Tabs,
      TabPane,
      [Button.name]: Button,
      [FormGroupInput.name]: FormGroupInput
    },
    head() {
        return {
            title: "%s | Services"
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