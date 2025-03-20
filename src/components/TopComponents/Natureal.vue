<script>
export default {
    name: "Natureal"
};
</script>

<template>
    <div class="relative z-[100] flex flex-col gap-[10px] w-[580px] top">
        <p class="font-[Inter-SemiBold] text-[82px] text-white opacity-[75%] p-0 m-0 h-[94px]">Breath Natural</p>
        <p class="font-[Inter-Medium] text-[18px] text-white opacity-[75%]">Lorem ipsum dolor sit amet, consectetur
            adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </p>

        <div class="flex items-center gap-[24px] block_">
            <button
                class="border-[2px] border-white/75 rounded-[13px] py-[6px] px-[48px] font-[Inter-Regular] text-[24px] text-white/75">Explore</button>

            <button class="border-[2px] border-white/75 rounded-full p-[10px] flex items-center justify-center"><img
                    src="/ui/play.png" alt="" class="w-[18px]"></button>

            <p class="font-[Inter-SemiBold] text-[18px] text-white opacity-[75%]">Live Demo...</p>
        </div>
    </div>
</template>

<style scoped>
@media screen and (max-width: 670px) {
    .top {
        width: 100%;
        padding: 0 20px;
    }

    .top p:nth-child(1){
        font-size: 60px;
        height: 70px;
    }

    .top p:nth-child(2){
        font-size: 16px;
    }
}

@media screen and (max-width: 462px) {
    .top p:nth-child(1){
        font-size: 44px;
        height: 50px;
    }

    .block_ button:nth-child(1){
        padding: 6px 16px;
    }

    .block_ p{
        font-size: 16px;
    }
}
</style>