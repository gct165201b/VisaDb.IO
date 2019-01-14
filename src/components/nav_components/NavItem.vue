<template>
    <li class="nav-item">
        <a class="nav-link" href="#"><i v-bind:class="navItem.icon"></i>  {{navItem.text}}</a>
    </li>
</template>

<script>
export default {
    name: 'NavItem',
    props:['navItem']
}
</script>

<style scoped>
    .navbar-dark .navbar-nav .nav-link {
        color: #fff;
    }

    .navbar-expand-lg .navbar-nav .nav-link {
        padding-left: 2.5rem;
    }
</style>






