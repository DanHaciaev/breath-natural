<template>
    <div class="flex flex-col items-center mt-[120px] mb-[160px] mx-[70px] best_">
        <div class="relative text-white text-[55px] font-[Inter-SemiBold] px-6 py-4 w-fit mb-[150px] zag">
            Our Best o2
            <div
                class="absolute right-0 top-0 w-[24px] h-[24px] bg-transparent border-r-[4px] border-t-[4px] border-[#50790B] rounded-tr-[12px]">
            </div>
            <div
                class="absolute left-0 bottom-0 w-[24px] h-[24px] bg-transparent border-l-[4px] border-b-[4px] border-[#50790B] rounded-bl-[12px]">
            </div>
        </div>


        <div
            class="relative border-2 min-h-[525px] border-white/25 rounded-[151px] pr-[120px] shadow-lg bg-white/15 flex justify-between w-full items-center best">
            <img src="/img/besto2.png" alt="" class="absolute bottom-0 left-[110px] plant">

            <div class="ml-auto w-[480px] space-y-4 text-white/75 text">
                <p class="font-[Inter-SemiBold] text-[28px]">We Have Small And Best O2 Plants Collection’s</p>

                <p class="font-[Inter-SemiBold] text-[20px]">Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                    sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua.
                </p>

                <p class="font-[Inter-SemiBold] text-[20px]">Lorem ipsum dolor sit amet, consectetur adipiscing elit,
                    sed do eiusmod tempor.</p>

                <div class="flex items-center justify-between">
                    <button
                        class="border-[2px] border-white/75 rounded-[13px] py-[4px] px-[32px] font-[Inter-Regular] text-[20px]">Explore</button>

                    <div class="flex items-center gap-[16px]">
                        <img src="/ui/left-arrow.png" alt="" class="w-[16px]">
                        <p class="font-[Inter-SemiBold] text-[20px]">01/<span class="text-[16px]">04</span></p>
                        <img src="/ui/right-arrow.png" alt="" class="w-[16px]">
                    </div>
                </div>
            </div>
        </div>

        <div class="flex gap-[10px] mt-[50px] justify-center">
            <div class="bg-white/75 w-[20px] h-[6px] rounded-[9px]"></div>
            <div class="bg-white/75 w-[6px] h-[6px] rounded-full"></div>
            <div class="bg-white/75 w-[6px] h-[6px] rounded-full"></div>
        </div>
    </div>
</template>

<style lang="css" scoped>
@media screen and (max-width: 1260px) {
    .best {
        height: fit-content;
        padding: 60px 30px 0;
        width: 600px;
        justify-content: space-between;
        align-items: center;
        gap: 30px;
        flex-direction: column-reverse;
    }

    .plant {
        position: unset;

    }

    .text {
        margin-left: 0;
    }
}

@media screen and (max-width: 769px) {
    .best_{
        margin: 80px 20px 160px;
    }
}

@media screen and (max-width: 620px) {
    .best {
        width: 100%;
        border-radius: 60px;
    }

    .zag{
        font-size: 36px;
        margin-bottom: 80px;
    }

    .text{
        width: 100%;
        margin: 0 20px;
    }

    .text p:nth-child(1) {
        font-size: 24px;
    }

    .text p:nth-child(2),
    .text p:nth-child(3) {
        font-size: 16px;
    }

    .plant {
        width: 250px;
    }
}

@media screen and (max-width: 380px) {
    .zag{
        font-size: 28px;
    }
}
</style>