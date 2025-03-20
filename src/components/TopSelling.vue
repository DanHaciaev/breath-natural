<script>
export default {
    name: "TopSelling"
};
</script>

<template>
    <div class="mt-[100px] flex flex-col justify-center mx-[70px] items-center top">
        <div class="relative text-white text-[55px] font-[Inter-SemiBold] px-6 py-4 w-fit mb-[40px] zag">
            Our Top Selling
            <div class="absolute right-0 top-0 w-[24px] h-[24px] bg-transparent border-r-[4px] border-t-[4px] border-[#50790B] rounded-tr-[12px]"></div>
            <div class="absolute left-0 bottom-0 w-[24px] h-[24px] bg-transparent border-l-[4px] border-b-[4px] border-[#50790B] rounded-bl-[12px]"></div>
        </div>

        <div class="flex flex-wrap gap-[24px] justify-center">
            <div class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[400px] px-[40px] flex justify-center mt-[80px] item">
                <div style="transform: translateY(-100px)" class="flex flex-col gap-[24px] items-center">
                    <img src="/img/calathea-plant.png" alt="Calathea plant" class="w-[340px] plant1" />
                    <div class="flex flex-col gap-[24px] text">
                        <p class="font-[Inter-Regular] text-[24px] text-white/75">Calathea plant</p>
                        <p class="font-[Inter-Regular] text-[20px] text-white/75">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                        <div class="flex items-center justify-between w-full">
                            <p class="font-[Inter-Regular] text-[24px] text-white/75">Rs. 309/-</p>
                            <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                                <img src="/ui/bag.png" alt="" class="w-[24px]">
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[400px] px-[40px] flex justify-center mt-[80px] item">
                <div style="transform: translateY(-80px)" class="flex flex-col gap-[24px] items-center">
                    <img src="/img/small-desk.png" alt="Desk plant" class="w-[380px] plant2" />
                    <div class="flex flex-col gap-[24px] text">
                        <p class="font-[Inter-Regular] text-[24px] text-white/75">Desk plant</p>
                        <p class="font-[Inter-Regular] text-[20px] text-white/75">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                        <div class="flex items-center justify-between w-full">
                            <p class="font-[Inter-Regular] text-[24px] text-white/75">Rs. 359/-</p>
                            <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                                <img src="/ui/bag.png" alt="" class="w-[24px]">
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[400px] px-[40px] flex justify-center mt-[80px] item">
                <div style="transform: translateY(-100px)" class="flex flex-col gap-[24px] items-center">
                    <img src="/img/calathea-ai.png" alt="Calathea ai plant" class="w-[170px] plant3" />
                    <div class="flex flex-col gap-[24px] text">
                        <p class="font-[Inter-Regular] text-[24px] text-white/75">Calathea ai plant</p>
                        <p class="font-[Inter-Regular] text-[20px] text-white/75">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                        <div class="flex items-center justify-between w-full">
                            <p class="font-[Inter-Regular] text-[24px] text-white/75">Rs. 399/-</p>
                            <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                                <img src="/ui/bag.png" alt="" class="w-[24px]">
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <div class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[400px] px-[40px] flex justify-center mt-[80px] item">
                <div style="transform: translateY(-100px)" class="flex flex-col gap-[24px] items-center">
                    <img src="/img/cal84.png" alt="Cal 874 plant" class="w-[180px] plant4" />
                    <div class="flex flex-col gap-[24px]">
                        <p class="font-[Inter-Regular] text-[24px] text-white/75">Cal 874 plant</p>
                        <p class="font-[Inter-Regular] text-[20px] text-white/75">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                        <div class="flex items-center justify-between w-full">
                            <p class="font-[Inter-Regular] text-[24px] text-white/75">Rs. 259/-</p>
                            <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                                <img src="/ui/bag.png" alt="" class="w-[24px]">
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[400px] px-[40px] flex justify-center mt-[80px] item">
                <div style="transform: translateY(-104px)" class="flex flex-col gap-[24px] items-center">
                    <img src="/img/besto2.png" alt="Show plant" class="w-[240px] plant5" />
                    <div class="flex flex-col gap-[24px]">
                        <p class="font-[Inter-Regular] text-[24px] text-white/75">Show plant</p>
                        <p class="font-[Inter-Regular] text-[20px] text-white/75">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                        <div class="flex items-center justify-between w-full">
                            <p class="font-[Inter-Regular] text-[24px] text-white/75">Rs. 759/-</p>
                            <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                                <img src="/ui/bag.png" alt="" class="w-[24px]">
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <div class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[400px] px-[40px] flex justify-center mt-[80px] item">
                <div style="transform: translateY(-104px)" class="flex flex-col gap-[24px] items-center">
                    <img src="/img/calat.png" alt="Show plant" class="w-[240px] plant6" />
                    <div class="flex flex-col gap-[24px]">
                        <p class="font-[Inter-Regular] text-[24px] text-white/75">Calat O2 plant</p>
                        <p class="font-[Inter-Regular] text-[20px] text-white/75">Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                        <div class="flex items-center justify-between w-full">
                            <p class="font-[Inter-Regular] text-[24px] text-white/75">Rs. 659/-</p>
                            <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                                <img src="/ui/bag.png" alt="" class="w-[24px]">
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
@media screen and (max-width: 769px) {
    .top {
        margin: 100px 20px 0;
    }
}

@media screen and (max-width: 620px) {
    .zag {
        font-size: 36px;
    }
}

@media screen and (max-width: 430px) {
    .item {
        width: 300px;
    }

    .plant1{
        width: 200px;
    }

    .plant2{
        width: 190px;
    }

    .plant3{
        width: 110px;
    }

    .plant4{
        width: 90px;
    }

    .plant5{
        width: 130px;
    }

    .plant6{
        width: 120px;
    }

    .text p:nth-child(1){
        font-size: 20px;
    }

    .text p:nth-child(2){
        font-size: 16px;
    }

    .text div p:nth-child(1){
        font-size: 20px;
    }
}

@media screen and (max-width: 380px) {
    .zag{
        font-size: 28px;
    }
}
</style>
