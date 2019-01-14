<template>
    <header>
        <Navigation />
    </header>
</template>

<script>
import Navigation from './Navigation.vue';
export default {
    name: 'Header',
    components: {
        Navigation
    }
}
</script>

<style scoped>

    header {
        height: 50px;
    }

</style>


