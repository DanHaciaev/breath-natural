<script>
export default {
    name: "Calathea"
};
</script>

<template>
    <div class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[410px] flex justify-center block_">
        <div class="-translate-y-[100px] flex flex-col gap-[24px]">
            <img src="/img/calathea-plant.png" alt="" class="w-[340px]">
            <div class="flex flex-col gap-[24px] pl-[16px]">
                <p class="font-[Inter-Regular] text-[20px] text-white">Trendy House Plant</p>
                <div class="flex items-center justify-between">
                    <p class="font-[Inter-Regular] text-[28px] text-white">Calathea plant</p>
                    <img src="/ui/right-arrow.png" alt="" class="w-[13px]">
                </div>
                <button
                    class="border-[2px] border-white/75 rounded-[13px] py-[6px] px-[32px] font-[Inter-Regular] text-[20px] text-white/75 w-fit">Buy
                    Now</button>
            </div>


            <div class="flex gap-[10px] justify-center">
                <div class="bg-white/75 w-[20px] h-[6px] rounded-[9px]"></div>
                <div class="bg-white/75 w-[6px] h-[6px] rounded-full"></div>
                <div class="bg-white/75 w-[6px] h-[6px] rounded-full"></div>
            </div>
        </div>
    </div>
</template>


<style scoped>
@media screen and (max-width: 450px) {
    .block_{
        width: 330px;
    }

    .block_ div img:nth-child(1){
        width: 250px;
    }
}

</style>
