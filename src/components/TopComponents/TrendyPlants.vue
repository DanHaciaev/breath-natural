<template>
    <div class="flex justify-center flex-col items-center px-[70px] w-full trendy">
        <div class="relative text-white text-[55px] font-[Inter-SemiBold] px-6 py-4 w-fit zag">
            Our Trendy Plants
            <div
                class="absolute right-0 top-0 w-[24px] h-[24px] bg-transparent border-r-[4px] border-t-[4px] border-[#50790B] rounded-tr-[12px]">
            </div>
            <div
                class="absolute left-0 bottom-0 w-[24px] h-[24px] bg-transparent border-l-[4px] border-b-[4px] border-[#50790B] rounded-bl-[12px]">
            </div>
        </div>

        <!-- Первый блок -->
        <div
            class="relative border-2 min-h-[406px] border-white/25 rounded-[151px] p-6 shadow-lg bg-white/15 flex justify-between w-full items-center mt-[170px] small-desk">
            <img src="/img/small-desk.png" alt="" class="absolute w-[520px] -translate-y-[130px] plant">
            <div class="ml-auto w-[600px] flex flex-col gap-[16px] text">
                <p class="text-[32px] font-[Inter-SemiBold] text-white">For Small Desk Ai Plant</p>
                <p class="text-[16px] font-[Inter-SemiBold] text-white">Lorem ipsum dolor sit amet, consectetur
                    adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
                <p class="text-[28px] font-[Inter-SemiBold] text-white">Rs. 599/-</p>
                <div class="flex items-center gap-[16px]">
                    <button
                        class="border-[2px] border-white rounded-[13px] py-[6px] px-[32px] font-[Inter-Regular] text-[20px] text-white w-fit">Buy
                        Now</button>
                    <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                        <img src="/ui/bag.png" alt="" class="w-[24px]">
                    </button>
                </div>
            </div>
        </div>

        <!-- Второй блок -->
        <div
            class="relative border-2 min-h-[406px] border-white/25 rounded-[151px] p-6 shadow-lg bg-white/15 flex justify-between w-full items-center mt-[170px] small-desk">
            <img src="/img/small-desk2.png" alt="" class="hidden w-[380px] -translate-y-[100px] right-[70px] plant__">
        
            <div class="ml-[73px] w-[600px] flex flex-col gap-[16px] text">
                <p class="text-[32px] font-[Inter-SemiBold] text-white">For Small Desk Ai Plant</p>
                <p class="text-[16px] font-[Inter-SemiBold] text-white">Lorem ipsum dolor sit amet, consectetur
                    adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
                <p class="text-[28px] font-[Inter-SemiBold] text-white">Rs. 599/-</p>
                <div class="flex items-center gap-[16px]">
                    <button
                        class="border-[2px] border-white rounded-[13px] py-[6px] px-[32px] font-[Inter-Regular] text-[20px] text-white w-fit">Buy
                        Now</button>
                    <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                        <img src="/ui/bag.png" alt="" class="w-[24px]">
                    </button>
                </div>
            </div>
            <img src="/img/small-desk2.png" alt="" class="absolute w-[380px] -translate-y-[100px] right-[70px] plant_">
        </div>
    </div>
</template>

<style scoped>
@media screen and (max-width: 1260px) {
    .small-desk {
        height: 600px;
        width: fit-content;
        align-items: center;
        justify-content: center;
        padding: 0 60px 40px;
    }

    .text {
        margin-left: 0;
        margin-top: auto;
        width: 450px;
    }

    .plant {
        transform: translateY(-20%);
    }

    .plant_ {
        transform: translateY(-25%) translateX(-7%);
        width: 360px;
    }
}

@media screen and (max-width: 769px) {
    .trendy {
        padding: 0 20px;
    }
}

@media screen and (max-width: 620px) {
    .zag{
        font-size: 36px;
    }
}

@media screen and (max-width: 600px) {
    .plant_{
        display: none;
    }

    .plant__{
        display: block;
        width: 250px;
        position: unset;
        transform: translateY(100px);
    }

    .plant{
        width: 300px;
        position: unset;
        transform: translateY(130px);
    }

    .text{
        width: 100%;
    }

    .small-desk{
        /* height: 550px; */
        margin-top: 50px;
        height: fit-content;
        border-radius: 70px;
        flex-direction: column;
        padding: 0 30px 40px;
        min-height: unset;
        position: unset;
    }
}

@media screen and (max-width: 380px) {
    .zag{
        font-size: 28px;
    }
}
</style>