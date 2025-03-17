<script>
export default {
    name: "Customer",
    data() {
        return {
            users: [
                {
                    name: "Maln Josi",
                    avatar: "/img/maln.png",
                    rating: 4.5,
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,"
                },
                {
                    name: "Alina Thakur",
                    avatar: "/img/thakur.png",
                    rating: 4.5,
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,"
                },
                {
                    name: "Max Makvana",
                    avatar: "/img/max.png",
                    rating: 4.5,
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,"
                }
            ]
        };
    },
    methods: {
        getFullStars(rating) {
            return Math.floor(rating);
        },
        hasHalfStar(rating) {
            return rating % 1 !== 0;
        }
    }
};
</script>

<template>
    <div class="flex flex-col items-center mt-[120px] mx-[70px]">
        <div class="relative text-white text-[55px] font-[Inter-SemiBold] px-6 py-4 w-fit mb-[150px]">
            Customer Review
            <div
                class="absolute right-0 top-0 w-[24px] h-[24px] bg-transparent border-r-[4px] border-t-[4px] border-[#50790B] rounded-tr-[12px]">
            </div>
            <div
                class="absolute left-0 bottom-0 w-[24px] h-[24px] bg-transparent border-l-[4px] border-b-[4px] border-[#50790B] rounded-bl-[12px]">
            </div>
        </div>
        <div class="flex justify-between w-full ">
            <div v-for="(user, index) in users" :key="index"
                class="top-120px bg-[url(/ui/customer.png)] bg-cover bg-no-repeat w-[500px] h-[350px] px-[50px] py-[60px]">
                <div class="flex items-center space-x-4">
                    <img :src="user.avatar" alt="User avatar" class="w-[60px] h-[60px] rounded-full">
                    <div>
                        <p class="text-[24px] font-[Inter-Medium] text-white">{{ user.name }}</p>
                        <div class="flex space-x-1 mt-1">
                            <img v-for="n in getFullStars(user.rating)" :key="n" src="/ui/star.png" alt="Star"
                                class="w-[15px]">
                            <img v-if="hasHalfStar(user.rating)" src="/ui/half_star.png" alt="Half Star"
                                class="w-[8px]">
                        </div>
                    </div>
                </div>
                <p class="mt-4 font-[Inter-Regular] text-white/75 text-[17px]">
                    {{ user.text }}
                </p>
            </div>
        </div>
    </div>

</template>
