<script setup>

import {ref} from "vue"


const cas = ref(10);

const odpocet = intevalCas (() => {
    if (cas.value < 0) {
        console.log(`${cas.value}`);
        cas.value--;        
    }else {
        console.log("HOTOVO!");
        clearInterval(intevalCas);
    }     
}, 1000);
</script>

<template>
    <p>: {{ cas }}</p>
</template>

<style soped>
    p {
        color: black
    }
</style>