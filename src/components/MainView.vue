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
    <div class="bg-[url('/img/back.png')] h-[1972px] min-h-screen bg-contain bg-no-repeat bg-bottom relative view">
        <Natureal class="absolute left-[70px] top-[110px] natureal" />
        <Calathea class="absolute right-[70px] top-[110px] calathea" />
        <Patel class="absolute left-[70px] top-[450px] patel" />
        <TrendyPlants class="absolute left-1/2 transform -translate-x-1/2 bottom-0 " />
    </div>
</template>

<style lang="css" scoped>
@media screen and (max-width: 1260px) {
    .view {
        height: 2400px;
        background-size: cover;
    }
}

@media screen and (max-width: 1150px) {
    .view {
        height: 3000px;
        background-size: cover;
    }

    .natureal {
        left: 20px;
    }

    .calathea {
        right: 20px;
        top: 440px;
    }

    .patel {
        left: 20px;
        top: 1050px;
    }
}

@media screen and (max-width: 769px) {
    .view {
        height: 2950px;
        background-size: cover;
    }

    .natureal {
        top: 50px;
        left: 50%;
        transform: translateX(-50%);
    }

    .calathea {
        left: 50%;
        transform: translateX(-50%);
        right: 0;
        top: 400px;
    }

    .patel {
        left: 50%;
        transform: translateX(-50%);
        top: 1000px;
    }

}

@media screen and (max-width: 600px) {
    .view {
        height: 2650px;
    }
}

@media screen and (max-width: 450px) {
    .patel{
        top: 850px;
    }
}
</style>
