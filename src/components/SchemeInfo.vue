<template>
    <div class="container mt-5">
        <div class="row">
            
                <HolVisReq text1="Holiday Visa Required" text2="Working Holiday Scheme"/>
                <EditVisInfo updated="Last Updated 2018-11-26 8:54pm" btnText="Add or correct info"/>
        </div>
        
    </div>
</template>


<script>
import HolVisReq from './scheme_info/HolidayVisaRequired';
import EditVisInfo from './scheme_info/EditVisaInfo';
export default {
    name: 'SchemeInfo',
    components: {
        HolVisReq,
        EditVisInfo
    }
}
</script>


