<template>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
            <NavItem v-bind:navItem="navItem" v-for="(navItem, index) in navItems" :key="index" v-if="navItem.align"/>
        </ul>

        <ul class="navbar-nav ml-auto">
            
            <NavItem v-bind:navItem="navItem" v-for="(navItem, index) in navItems" :key="index" v-if="!navItem.align"/>
            
        </ul>
    </div>
    
</template>

<script>
import NavItem from './NavItem'
export default {
    name: 'Navbar',
    components: {
        NavItem
    },
    props: ["navItems"]
}
</script>

