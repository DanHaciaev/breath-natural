<template>
    <div class="mx-[70px] mb-[80px] top_">
        <div class="flex justify-between items-start top">
            <div class="w-[500px] space-y-4 text_top">
                <div class="flex items-center gap-[8px]">
                    <img src="/img/plant_header.png" alt="" class="w-[48px]">
                    <p class="font-[Inter-Black] text-[28px] text-white">Planto.</p>
                </div>
                <p class="font-[Inter-Medium] text-[24px] text-white">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua.
                </p>
            </div>

            <div class="flex flex-col gap-[40px]">
                <p class="font-[Inter-SemiBold] text-[24px] text-white/75">Quick Link’s</p>
                <ul class="flex flex-col gap-[8px] p-0 text-white/75 text-[20px] font-[Inter-Medium]">
                    <li>Home</li>
                    <li class="flex items-center gap-[4px]">Category <img src="/ui/arrow-down.png" alt=""
                            class="w-[12px]"></li>
                    <li>More</li>
                    <li>Contact</li>
                </ul>
            </div>

            <div class="flex flex-col gap-[40px] relative">
                <p class="font-[Inter-SemiBold] text-[24px] text-white/75">For Every Update’s</p>

                <label class="w-fit h-[50px] label_">
                    <input class="border-[2px] pl-[16px] w-[220px] border-white rounded-l-[10px] h-full font-[Inter-SemiBold] text-white" type="text" placeholder="Enter Email...">
                    <button class="bg-white h-full px-[16px] rounded-r-[10px]">SUBSCRIBE</button>
                </label>

                <p class="absolute top-[280px] font-[Inter-SemiBold] text-[20px] text-white/75 text_">Planto © All right reserve</p>
            </div>
        </div>

        <div class="flex justify-between mt-[60px]">
            <ul class="flex gap-[57px] font-[Inter-SemiBold] text-[24px] text-white">
                <li>FB</li>
                <li>TW</li>
                <li>LI</li>
            </ul>

            
        </div>
    </div>
</template>

<style scoped>
    @media screen and (max-width: 1200px) {
        .top{
            gap: 24px;
            flex-wrap: wrap;
        }
    }

    @media screen and (max-width: 769px) {
        .top{
            flex-direction: column;
            justify-content: center;
        }

        .top_{
            flex-direction: column;
            display: flex;
            justify-content: center;
            margin: 0 20px 80px;
        }

        .text_{
            position: unset;
        }

        .text_top{
            width: 100%;
        }
    }

    @media screen and (max-width: 390px) {
        .label_{
            width: 335px;
        }
    }
</style>