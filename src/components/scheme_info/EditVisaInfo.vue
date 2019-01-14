<template>
    <div class="col-md-6 col-sm-12">
        <div class="float-md-right">
            <span class="text-right">
                {{updated}}
            </span>
            <button class="btn btn-outline-primary mt-3">
                <i class="fas fa-pen"></i>  
                {{btnText}}
            </button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'EditVisInfo',
    props: {
        updated: String,
        btnText: String
    }
}
</script>

<style scoped>
    span {
        font-size: 15px;
        color: #86888C;
    }
    .btn {
        display: block;
        font-style: normal;
        font-weight: bold;
        font-size: 15px;
        border-radius: 0;
    }

</style>
