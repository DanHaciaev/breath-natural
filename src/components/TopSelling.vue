<script>
export default {
    name: "TopSelling",
    data() {
        return {
            topSellingPlants: [
                {
                    name: "Calathea plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
                    price: "Rs. 309/-",
                    image: "/img/calathea-plant.png",
                    imgWidth: "340px",
                    translateY: "100px"
                },
                {
                    name: "Desk plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
                    price: "Rs. 359/-",
                    image: "/img/small-desk.png",
                    imgWidth: "380px",
                    translateY: "80px"
                },
                {
                    name: "Calathea ai plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
                    price: "Rs. 399/-",
                    image: "/img/calathea-ai.png",
                    imgWidth: "170px",
                    translateY: "100px"
                },
                {
                    name: "Cal 874 plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
                    price: "Rs. 259/-",
                    image: "/img/cal84.png",
                    imgWidth: "180px",
                    translateY: "100px"
                },
                {
                    name: "Show plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
                    price: "Rs. 759/-",
                    image: "/img/besto2.png",
                    imgWidth: "240px",
                    translateY: "104px"
                },
                {
                    name: "Calat O2 plant",
                    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit",
                    price: "Rs. 659/-",
                    image: "/img/calat.png",
                    imgWidth: "240px",
                    translateY: "105px"
                }
            ]
        };
    }
};
</script>

<template>
    <div class="mt-[100px] flex flex-col justify-center mx-[70px] items-center">
        <div class="relative text-white text-[55px] font-[Inter-SemiBold] px-6 py-4 w-fit mb-[40px]">
            Our Top Selling
            <div class="absolute right-0 top-0 w-[24px] h-[24px] bg-transparent border-r-[4px] border-t-[4px] border-[#50790B] rounded-tr-[12px]"></div>
            <div class="absolute left-0 bottom-0 w-[24px] h-[24px] bg-transparent border-l-[4px] border-b-[4px] border-[#50790B] rounded-bl-[12px]"></div>
        </div>

        <div class="flex flex-wrap justify-between">
            <div v-for="(plant, index) in topSellingPlants" :key="index"
                class="top-120px bg-[url(/ui/green-back.png)] bg-contain bg-no-repeat w-[410px] px-[40px] flex justify-center mt-[80px]">
                
                <div :style="{ transform: `translateY(-${plant.translateY})` }" class="flex flex-col gap-[24px] items-center">
                    <img :src="plant.image" :alt="plant.name" :style="{ width: plant.imgWidth }" />
                    
                    <div class="flex flex-col gap-[24px]">
                        <p class="font-[Inter-Regular] text-[24px] text-white/75">{{ plant.name }}</p>
                        <p class="font-[Inter-Regular] text-[20px] text-white/75">{{ plant.description }}</p>

                        <div class="flex items-center justify-between w-full">
                            <p class="font-[Inter-Regular] text-[24px] text-white/75">{{ plant.price }}</p>
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