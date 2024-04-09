<script lang="ts">

import SectionIntro from '../../text/sectionIntro.vue';
import UserReviewCard from '../../card/userReviewCard.vue';

export default defineComponent({
    name: "Comments",
    components: {
        SectionIntro,
        UserReviewCard
    },
    data() {
        return {
            review: "همیشه وقتی وسایل تو یخچالم داره خراب میشه به این فکر میکنم که کاش میتونستم یه چیزی با همین وسایل درست کنم که هم مواد غذایی خراب نشه و هم غذای خونگی بخورم. ولی پیدا کردن ایده همیشه کار سختی بود. برای همین فودی رو درست کردم تا نه تنها مشکل خودمو حل کنم، بلکه به بقیه آدمایی که هر روز سوال چی بپزم رو از خودشون یا اطرافیانشون می‌پرسن هم کمک کنم ❤️",
            name: 'فاطمه',
            imagePath: '/assets/images/user.jpg'
            // 
        }
    }

});
</script>



<template>
    <div class="section-container wsm:flex-col gap-x-10 relative items-center">

        <div class="flex flex-col w-full">

            <SectionIntro title="بقیه چی میگن؟" />

            <h2 class="text-[#031837] font-bold wsm:text-3xl text-[55px]  py-8 leading-[65px]">
                ببینیم بقیه نظرشون <br>
                درباره اپ چـیـــــــــه ؟
            </h2>
            <UserReviewCard
                :review="review"
                :name="name" :imagePath="imagePath" />
        </div>
        <div class="flex w-full wsm:hidden">
            <img src="/public/assets/images/cookingFood.jpg" class="w-[100%] rounded-3xl" alt="">
        </div>
    </div>
</template>
