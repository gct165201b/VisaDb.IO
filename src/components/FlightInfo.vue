<template>
    <div class="container-fluid">
        <div class="text-center">
            <span>
                <img class="flag" v-bind:src="this.countries[0].flag" alt="">
                <label class="visa-text">{{this.countries[0].name}}</label>
            </span>

            <img src="../assets/plan.svg" alt="">

            <span class="visa">
                <span>Holiday</span> Visa
            </span>

            <span>
                <label class="visa-text">{{this.countries[1].name}}</label>
                <img class="flag" v-bind:src="this.countries[1].flag" alt="">
            </span>

            <span class="close float-right">&times;</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FlightInfo',
    data() {
        return {
            countries: [
                {
                    name: 'Canada',
                    flag: 'https://lipis.github.io/flag-icon-css/flags/4x3/ca.svg'
                },

                {
                    name: 'South Korea',
                    flag: 'https://lipis.github.io/flag-icon-css/flags/4x3/kr.svg'
                }
            ]
        }
    }
}
</script>

<style scoped>
    .container-fluid {
        background: #CDCDCD;
        margin-top: -3px;
    }

    .container-fluid div {
        height: 100%;
        line-height: 100%;
        padding: 10px 0;
    }

    .flag {
        height: 30px;
        width: 30px;
        margin: 0 10px;
    }

    .visa-text {
        font-family: 'Quicksand';
        font-style: normal;
        font-weight: normal;
        line-height: normal;
        font-size: 25px;
        color: #86888C;
        text-decoration: underline;
        margin: 0 10px;
    }

    .visa {
        margin: 0 10px;
        background: #fff;
        color: #0150B1;
        padding: 5px;
    }

    .visa span {
        font-weight: bold;
    }

    .close {
        font-size: 30px;
    }
</style>

