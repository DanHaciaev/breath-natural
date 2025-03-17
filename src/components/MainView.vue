<script>
import Natureal from './TopComponents/Natureal.vue';
import Calathea from './TopComponents/Calathea.vue';
import Patel from './TopComponents/Patel.vue';
import TrendyPlants from './TopComponents/TrendyPlants.vue';

export default {
    components: {
        Natureal,
        Calathea,
        Patel,
        TrendyPlants
    }
};
</script>

<template>
    <div class="bg-[url('/img/back.png')] h-[1972px] min-h-screen bg-cover bg-bottom relative">
        <Natureal class="absolute left-[70px] top-[110px]"/>
        <Calathea class="absolute right-[70px] top-[110px]"/>
        <Patel class="absolute left-[70px] top-[450px]"/>
        <TrendyPlants class="absolute left-1/2 transform -translate-x-1/2 bottom-0"/>
    </div>
</template>
