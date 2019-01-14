<template>
    <div class="container mt-4">

        <div class="row">
            <AboutVisLeft v-bind:aboutVisLeft="this.aboutVisLeft"/>

            <div class="col-md-auto col-sm-auto line mt-3"></div>

            <AboutVisRight v-bind:abouts="this.abouts"/>
        </div>

    </div>
</template>

<script>

import AboutVisLeft from './about_visa/AboutVisaLeft.vue';
import AboutVisRight from './about_visa/AboutVisaRight.vue';

export default {
    name: 'AboutVisa',
    components: {
        AboutVisLeft,
        AboutVisRight
    },
    data() {
        return {
            aboutVisLeft: {
                header : 'About this visa',
                p: `You can enjoy holidays in the Republic of Korea by applying Working Holiday Visa at the embassy of the republic of Korea. Working Holiday Visa allows <strong>young people to travel and work</strong> in the Republic of Korea for <strong>12 months (maximum)</strong>. The main purpose of this program is to enable the young people to have an extended holiday while supplementing necessary funds with short-term work in the Republic of Korea.`
            },
            abouts : [
                {
                    text : `DURATION: <strong>12 MONTHS</strong>`,
                    icon: 'fas fa-calendar-alt'
                },
                {
                    text : `FEES: <strong>90$ VISA</strong>`,
                    icon: 'fas fa-money-bill-alt'
                },
                {
                    text : `COMPLEXITY: <strong>VERY LOW</strong>`,
                    icon: 'fas fa-puzzle-piece'
                }
            ]
        }
    }
}
</script>

<style scoped>
    .container {
        border: 1px solid #C4C4C4;
    }
    
    .line {
        height: 140px;
        width: 0px;
        border: 1px solid #C4C4C4;
        padding: 0;
    }
    
</style>

