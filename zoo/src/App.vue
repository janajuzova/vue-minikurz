<script setup>
import PocetNavstevniku from './components/PocetNavstevniku.vue';
import Ukol10odpocitavadlo from './components/Ukol10odpocitavadlo.vue';
import ComputedPromenna from './components/ComputedPromenna.vue';
import DirektivaOn from './components/DirektivaOn.vue';
import DirektivaBind from './components/DirektivaBind.vue';
import DirektivaShowIf from './components/DirektivaShowIf.vue';
</script>


<template>
  <div class="container">
    <h1>Zoo</h1>
    <p class="uvod">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Qui repellat quos, error necessitatibus itaque dignissimos sit, libero debitis est facilis, recusandae delectus voluptate iure maxime. Est quam aperiam incidunt iure.</p>

    <div class="karta">
      <PocetNavstevniku />
    </div>

    <h2>Ukol 10 ODPOCITAVADLO</h2>

    <div class="karta">
      <Ukol10odpocitavadlo />
    </div> 

    <div class="karta">
      <ComputedPromenna />
    </div>

    <div class="karta">
      <DirektivaOn />
    </div>

    <div class="karta">
      <DirektivaBind />
    </div>

    <div class="karta">
      <DirektivaShowIf />
    </div>

  </div>
</template>

<style scoped>
    h1 {
      color: cadetblue;
      text-align: center;
    }

    h2 {
      color: blue;
      text-align: center;
    }

    p.uvod {
      text-align: center;
      font-size: 1.5rem;
      font-weight: bold;
    }

    .karta {
      background-color: coral;
      border-radius: 10px;
      margin: 1rem;
      padding: 2rem;
      font-size: 1.1rem;
      color: white;
    }
</style>