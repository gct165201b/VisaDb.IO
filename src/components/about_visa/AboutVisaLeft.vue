<template>
    <div class="col-md-8 col-sm-8">
        <h3 v-text="aboutVisLeft.header"></h3>

        <p v-html="aboutVisLeft.p">
        </p>
    </div>
</template>

<script>
export default {
    name: 'AboutVisLeft',
    props : [
        "aboutVisLeft"
    ]
}
</script>

<style scoped>
    h3 {
        /* About this visa */

        font-weight: bold;
        font-size: 20px;
        color: #0150B1;
        padding: 3px 5px;
    }
    p {
        padding: 3px 5px;
        text-align: justify;
    }
</style>

