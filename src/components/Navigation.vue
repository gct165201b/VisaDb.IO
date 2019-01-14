<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-light">
        <a class="navbar-brand" href="#">
            <!-- LOGO -->
            <img class="logo" src="../assets/logo.png" alt="LOGO"> 
        </a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>

        
            <Navbar v-bind:navItems="navItems"/>
        
    </nav>
</template>

<script>
import Navbar from './nav_components/Navbar.vue';
export default {
    name: 'Navigation',
    components: {
        Navbar
    },
    data() {
        return {
            navItems: [
                {
                    text: 'Search',
                    href: '#',
                    icon: 'fas fa-search',
                    align: true
                },
                {
                    text: 'Passport Ranking',
                    href: '#',
                    icon: 'fas fa-passport',
                    align: true
                },
                {
                    text: 'Partner',
                    href: '#',
                    icon: 'fas fa-hands-helping',
                    align: true
                },
                {
                    text: 'News',
                    href: '#',
                    icon: 'far fa-newspaper',
                    align: true
                },
                {
                    text: 'Contact Us',
                    href: '#',
                    icon: 'fas fa-envelope',
                    align: true
                },
                {
                    text: 'More',
                    href: '#',
                    icon: 'fas fa-ellipsis-h',
                    align: true
                },
                {
                    text: 'Login',
                    href: '#',
                    icon: 'far fa-user',
                    align: false
                },
                {
                    text: 'Select Language',
                    href: '#',
                    icon: 'fas fa-caret-down',
                    align: false
                }
            ]
        }
    }
}
</script>

<style scoped>
    .logo {
        width: 150px;
        height: auto;
        opacity: 0.5;
    }

    .navbar {
        padding: 0;
        margin: 0;
    }

    .bg-light {
        background-color: #0150B1!important;
    }
</style>

