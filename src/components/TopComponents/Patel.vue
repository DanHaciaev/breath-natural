<script>
export default {
    name: "Patel",
    data() {
        return {
            user: {
                name: "Alina Patel",
                avatar: "/img/alina.png",
                rating: 4.5
            }
        };
    },
    computed: {
        fullStars() {
            return Math.floor(this.user.rating);
        },
        halfStar() {
            return this.user.rating % 1 !== 0;
        }
    }
};
</script>

<template>
    <div class="border-2 border-white/25 rounded-3xl p-6 w-96 shadow-lg bg-white/15 block_">
        <div class="flex items-center space-x-4 ">
            <img :src="user.avatar" alt="User avatar" class="w-[60px] h-[60px] rounded-full">
            <div>
                <p class="text-[24px] font-[Inter-Medium] text-white">{{ user.name }}</p>
                <div class="flex space-x-1 mt-1">
                    <img v-for="n in fullStars" :key="n" src="/ui/star.png" alt="Star" class="w-[15px] ">
                    <img v-if="halfStar" src="/ui/half_star.png" alt="Half Star" class="w-[8px]">
                </div>
            </div>
        </div>
        <p class="mt-4 font-[Inter-Regular] text-white/75 text-[17px]">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt...
        </p>
    </div>
</template>

<style>
@media screen and (max-width: 450px) {
    .block_{
        width: 330px;
    }
}
</style>