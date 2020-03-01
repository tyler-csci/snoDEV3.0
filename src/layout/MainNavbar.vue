<template>
    <navbar position="fixed"
            :transparent="transparent"
            :color-on-scroll="colorOnScroll"
            menu-classes="ml-auto">
        <template>
                <a href="/">
                    <img src="/icon.png" width="60" height="40" alt="snoDEV logo">
                </a>
                <el-popover
                        ref="popover1"
                        popper-class="popover"
                        placement="bottom"
                        width="200"
                        trigger="hover">
                    <div class="popover-body">Designed by Invision. Coded by Creative Tim</div>
                </el-popover>
        </template>
        <template slot="navbar-menu">
            <ul class="navbar-nav mx-auto">
                <li class="nav-item category">
                    <a href="/" class="nav-link">
                        Home
                    </a>
                </li>
                <li class="nav-item">
                    <a href="/services" class="nav-link category">
                        Services
                    </a>
                </li>
                <li class="nav-item">
                    <a href="/showcase" class="nav-link category" >
                        Showcase
                    </a>
                </li>
                <li class="nav-item">
                    <a href="/about" class="nav-link category">
                        About
                    </a>
                </li>
                <li class="nav-item">
                    <a href="/blog-posts" class="nav-link category">
                        Blog
                    </a>
                </li>
                <li class="nav-item">
                    <a href="/contact" class="nav-link category">
                        Contact
                    </a>
                </li>
            </ul>
        </template>
    </navbar>
</template>

<script>
  import { DropDown, NavbarToggleButton, Navbar, NavLink } from '@/components';
  import { Popover } from 'element-ui'
  export default {
    name: 'main-navbar',
    props: {
      transparent: Boolean,
      colorOnScroll: Number,
    },
    components: {
      DropDown,
      Navbar,
      NavbarToggleButton,
      NavLink,
      [Popover.name]: Popover
    }
  }
</script>

<style scoped>

</style>
