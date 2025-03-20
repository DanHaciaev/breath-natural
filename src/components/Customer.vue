<template>
    <div class="flex flex-col items-center mt-[80px] mx-[40px] review">
        <div class="relative text-white text-[48px] font-[Inter-SemiBold] px-4 py-3 w-fit mb-[100px] zag">
            Customer Review
            <div
                class="absolute right-0 top-0 w-[20px] h-[20px] bg-transparent border-r-[3px] border-t-[3px] border-[#50790B] rounded-tr-[10px]">
            </div>
            <div
                class="absolute left-0 bottom-0 w-[20px] h-[20px] bg-transparent border-l-[3px] border-b-[3px] border-[#50790B] rounded-bl-[10px]">
            </div>
        </div>

        <!-- Для экранов < 945px -->
        <swiper v-if="windowWidth <= 1070" :modules="swiperModules" :slides-per-view="1" :space-between="10"
            :scrollbar="{ draggable: true, hide: true }" :style="{ paddingBottom: '40px' }" :loop="true"
            class="w-[90%]">
            <swiper-slide v-for="(user, index) in users" :key="index">
                <div
                    class="border-2 border-white/25 rounded-[84px] max-w-[440px] bg-white/15 px-[30px] py-[30px] mx-auto">
                    <div class="flex items-center space-x-3">
                        <img :src="user.avatar" alt="User avatar" class="w-[50px] h-[50px] rounded-full">
                        <div>
                            <p class="text-[22px] font-[Inter-Medium] text-white">{{ user.name }}</p>
                            <div class="flex space-x-1 mt-1">
                                <img v-for="n in getFullStars(user.rating)" :key="n" src="/ui/star.png" alt="Star"
                                    class="w-[14px]">
                                <img v-if="hasHalfStar(user.rating)" src="/ui/half_star.png" alt="Half Star"
                                    class="w-[7px]">
                            </div>
                        </div>
                    </div>
                    <p class="mt-3 font-[Inter-Regular] text-white/75 text-[16px]">
                        {{ user.text }}
                    </p>
                </div>
            </swiper-slide>
        </swiper>

        <!-- Для экранов 946px - 1390px -->
        <swiper v-else-if="windowWidth <= 1390" :modules="swiperModules" :slides-per-view="2" :space-between="20"
            :scrollbar="{ draggable: true, hide: true }" :loop="true" :style="{ paddingBottom: '40px' }"
            class="w-[90%]">
            <swiper-slide v-for="(user, index) in users" :key="index">
                <div
                    class="border-2 border-white/25 rounded-[84px] bg-white/15 px-[40px] py-[50px] mx-auto">
                    <div class="flex items-center space-x-3">
                        <img :src="user.avatar" alt="User avatar" class="w-[50px] h-[50px] rounded-full">
                        <div>
                            <p class="text-[22px] font-[Inter-Medium] text-white">{{ user.name }}</p>
                            <div class="flex space-x-1 mt-1">
                                <img v-for="n in getFullStars(user.rating)" :key="n" src="/ui/star.png" alt="Star"
                                    class="w-[14px]">
                                <img v-if="hasHalfStar(user.rating)" src="/ui/half_star.png" alt="Half Star"
                                    class="w-[7px]">
                            </div>
                        </div>
                    </div>
                    <p class="mt-3 font-[Inter-Regular] text-white/75 text-[16px]">
                        {{ user.text }}
                    </p>
                </div>
            </swiper-slide>
        </swiper>

        <!-- Для экранов > 1390px -->
        <div v-else class="flex justify-center space-x-6 w-[90%]">
            <div v-for="(user, index) in users" :key="index"
                class="border-2 border-white/25 rounded-[84px] bg-white/15 px-[40px] py-[50px]">
                <div class="flex items-center space-x-3">
                    <img :src="user.avatar" alt="User avatar" class="w-[50px] h-[50px] rounded-full">
                    <div>
                        <p class="text-[22px] font-[Inter-Medium] text-white">{{ user.name }}</p>
                        <div class="flex space-x-1 mt-1">
                            <img v-for="n in getFullStars(user.rating)" :key="n" src="/ui/star.png" alt="Star"
                                class="w-[14px]">
                            <img v-if="hasHalfStar(user.rating)" src="/ui/half_star.png" alt="Half Star"
                                class="w-[7px]">
                        </div>
                    </div>
                </div>
                <p class="mt-3 font-[Inter-Regular] text-white/75 text-[16px]">
                    {{ user.text }}
                </p>
            </div>
        </div>
    </div>
</template>

<style scoped>
@media screen and (max-width: 769px) {
    .review {
        margin: 80px 20px 0;
    }
}

@media screen and (max-width: 620px) {
    .zag {
        font-size: 36px;
    }
}

@media screen and (max-width: 380px) {
    .zag{
        font-size: 28px;
    }
}
</style>

<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Scrollbar } from 'swiper/modules';
import 'swiper/css';
import 'swiper/css/scrollbar';

export default {
    name: "Customer",
    components: {
        Swiper,
        SwiperSlide,
    },
    data() {
        return {
            windowWidth: window.innerWidth,
            swiperModules: [Scrollbar],
            users: [
                { name: "Maln Josi", avatar: "/img/maln.png", rating: 4.5, text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam," },
                { name: "Alina Thakur", avatar: "/img/thakur.png", rating: 4.5, text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam," },
                { name: "Max Makvana", avatar: "/img/max.png", rating: 4.5, text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam," }
            ]
        };
    },
    methods: {
        getFullStars(rating) {
            return Math.floor(rating);
        },
        hasHalfStar(rating) {
            return rating % 1 !== 0;
        },
        updateWindowWidth() {
            this.windowWidth = window.innerWidth;
        }
    },
    mounted() {
        window.addEventListener('resize', this.updateWindowWidth);
    },
    beforeUnmount() {
        window.removeEventListener('resize', this.updateWindowWidth);
    }
};
</script>
