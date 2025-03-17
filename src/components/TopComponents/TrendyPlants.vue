<script>
export default {
    name: "TrendyPlants",
    data() {
        return {
            plants: [
                {
                    title: "For Small Desk Ai Plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
                    price: "Rs. 599/-",
                    image: "/img/small-desk.png",
                    imagePosition: "left"
                },
                {
                    title: "For Small Desk Ai Plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua",
                    price: "Rs. 599/-",
                    image: "/img/small-desk2.png",
                    imagePosition: "right"
                }
            ]
        };
    }
};
</script>

<template>
    <div class="flex justify-center flex-col items-center px-[70px] w-full">
        <div class="relative text-white text-[55px] font-[Inter-SemiBold] px-6 py-4 w-fit">
            Our Trendy Plants
            <div class="absolute right-0 top-0 w-[24px] h-[24px] bg-transparent border-r-[4px] border-t-[4px] border-[#50790B] 
                rounded-tr-[12px]">
            </div>
            <div
                class="absolute left-0 bottom-0 w-[24px] h-[24px] bg-transparent border-l-[4px] border-b-[4px] border-[#50790B] 
                rounded-bl-[12px]">
            </div>
        </div>

        <div v-for="(plant, index) in plants" :key="index" 
            class="relative border-2 min-h-[406px] border-white/25 rounded-[151px] p-6 shadow-lg bg-white/15 flex justify-between w-full items-center mt-[170px] first:mt-0">
            
            <img v-if="plant.imagePosition === 'left'" :src="plant.image" alt="" class="absolute w-[520px] -translate-y-[130px]">
            
            <div :class="plant.imagePosition === 'right' ? 'ml-[73px]' : 'ml-auto'" class="w-[600px] flex flex-col gap-[16px]">
                <p class="text-[32px] font-[Inter-SemiBold] text-white">{{ plant.title }}</p>
                <p class="text-[16px] font-[Inter-SemiBold] text-white">{{ plant.description }}</p>
                <p class="text-[28px] font-[Inter-SemiBold] text-white">{{ plant.price }}</p>
                
                <div class="flex items-center gap-[16px]">
                    <button
                    class="border-[2px] border-white rounded-[13px] py-[6px] px-[32px] font-[Inter-Regular] text-[20px] text-white w-fit">Buy
                    Now</button>
                    <button class="border-[2px] border-white rounded-[13px] p-[8px]">
                        <img src="/ui/bag.png" alt="" class="w-[24px]">
                    </button>
                </div>
            </div>
            
            <img v-if="plant.imagePosition === 'right'" :src="plant.image" alt="" class="absolute w-[380px] -translate-y-[100px] right-[70px]">
        </div>
    </div>
</template>
