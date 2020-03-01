<template>
    <footer class="footer"
            :class="{[`footer-${type}`]: type}"
            :data-background-color="backgroundColor">
        <div class="container">
            <nav>
                <ul>
                    <li>
                        <a href="https://www.creative-tim.com">
                            snoDEV
                        </a>
                    </li>
                    <li>
                        <a href="https:///presentation.creative-tim.com">
                            About Us
                        </a>
                    </li>
                    <li>
                        <a href="https:///blog.creative-tim.com">
                            Contact
                        </a>
                    </li>
                    <li>
                        <a href="https://app.termly.io/document/privacy-policy/406ff816-5739-4921-8706-ff7f1182ccf1" rel="noopener" target="_blank">
                            Privacy Policy
                        </a>
                    </li>
                </ul>
            </nav>
            <div class="copyright">snoDEV
                &copy; {{year}}, using <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue.js</a>.
            </div>
        </div>
    </footer>
</template>
<script>
  export default {
    props: {
      backgroundColor: String,
      type: String
    },
    data(){
      return {
        year: new Date().getFullYear()
      }
    }
  }
</script>
<style>
</style>
