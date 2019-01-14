<template>
    <div class="col-md-6 col-sm-12">
        <span class="span-bg-red text-right">
            {{this.text1}}
        </span>

        <h1 class="text-red">
            {{this.text2}}
        </h1>

    </div>   
</template>

<script>
export default {
    name: 'HolVisReq',
    props: {
        text1: String,
        text2: String
    }
}
</script>


<style scoped>
    .span-bg-red {
        /* Holiday visa required */
        display: inline-block;
        background: #FF0935;
        padding: 2px 10px;
        font-family: Quicksand;
        font-style: normal;
        font-weight: bold;
        font-size: 20px;
        color: #FFFFFF;
    }

    h1 {
        width: 467px;
        height: 38px;
        padding: 5px 0;
        font-style: normal;
        font-weight: normal;
        line-height: normal;
        font-size: 30px;
        letter-spacing: 0.1em;
        text-transform: uppercase;
        color: #FF0935;
    }

</style>

