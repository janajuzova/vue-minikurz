<script setup>

import {ref} from "vue"


const cas = ref(10);

const odpocet = intevalCas (() => {
    cas.value--; 
}, 1000);


    if (cas < 0) {
        console.log("Hotovo");
        clearInterval(intevalCas);
    }


</script>

<template>
    <p>: {{ cas }}</p>
</template>

<style soped>
    p {
        color: black
    }
</style>