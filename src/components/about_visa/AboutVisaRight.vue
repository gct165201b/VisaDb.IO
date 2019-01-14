<template>
    <div class="col-md-3 col-sm-3">
        <div class="my-container mt-4">
            <span class="text" v-for="(about, index) in abouts" :key="index">
                <i v-bind:class="about.icon"></i>
                <span v-html="about.text">
                </span>
            </span>
        </div>
    </div>
</template>


<script>
export default {
    name: 'AboutVisRight',
    props: ['abouts']
}
</script>


<style scoped>
    .my-container {
        padding: 10px;
        width: 100%;
    }

    .text {
        display: block;
        color: #027BE3;
        padding: 5px;
    }

    .text i {
        padding-right: 5px;
    }
</style>

