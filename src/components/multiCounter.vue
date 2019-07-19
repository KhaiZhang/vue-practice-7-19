<template>
    <div>  
        <input v-model.number=" count" placeholder="edit me " id="input">
        <count v-for="item in count" :key="item.id"></count>
    </div>
</template>
<script>
    import count from './count.vue'
    export default {
    name: 'multicounter',
    components :{
        count
    },
    props: {
        msg: String
    },
    data(){
        return{
            count:0
        } 
    },
    }
</script>

<style>
</style>