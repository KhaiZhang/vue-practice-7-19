<template>
    <div id="container">
        <button @click="up">+</button>
        <span id="content">{{count}}</span>
        <button @click="down">-</button>
    </div>
</template>
<script>
    export default {
    name: 'count',
    props: {
        msg: String
    },
    data(){
        return{
            count:0
        } 
    },
    methods:{
        up:function(event){
            this.count++;
        },
        down:function(event){
            this.count--;
        }
    }
    }
</script>
<style>
    button {
        margin: 25px;
    }
</style>
