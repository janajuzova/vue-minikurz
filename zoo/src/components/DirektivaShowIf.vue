<script setup>
import {computed, ref} from "vue"

const zobrazitDiv = ref(false);
const textTlacitka = computed(() => {
    if (zobrazitDiv.value) {
        return "Skrt text";
    }else {
        return "Zobrazit text"
    }
});

const cislo = ref(0);

</script>

<template>
    <h2>Direktiva v-show a v-if</h2>

    <button @click="zobrazitDiv=!zobrazitDiv">{{ textTlacitka }}</button>
    <div v-show="zobrazitDiv">
        <p>skryta zprava!!!</p>
    </div>

    <div>
        <p>Stav pocitadla: {{ cislo }}</p>
        <button @click="cislo++">Zvednout</button>
    </div>
    <h4 v-if="cislo < 5">Cislo je male</h4>
    <h3 v-else-if="cislo < 10">Cislo je stredne velke</h3>
    <h2 v-else >Cislo je velke</h2>

</template>

<style scoped>
</style>