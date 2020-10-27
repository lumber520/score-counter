<template>
    <div>
        <h2> {{name}}</h2>
        <p>{{player.score}}</p>
        <button @click="decrease">
            Decrease
        </button>
        <button @click="increase">
            Increase
        </button>
    </div>
</template>

<script setup>
    import {  reactive } from 'vue'
export default {

    props:{
        name:String,
    },
    inheritAttrs:false
};
    export const player = reactive( {
        score: 0,
    });
    export const increase = () =>{
        player.score++
    };
    export  const decrease = () =>{
        player.score--
    }
</script>


<style scoped>

</style>