<script lang="ts">

import SectionIntro from '../../text/sectionIntro.vue';
import AboutUsCard from '../../card/aboutUsCard.vue';

interface CardData {
    imagePath: string;
    title: string;
    category: string;
}

export default defineComponent({
    name: "AboutUs",
    components: {
        SectionIntro,
        AboutUsCard
    },
    data() {
        return {
            cardData: [
                {
                    imagePath: '/assets/images/card/breakfast.jpg',
                    title: 'پنکیک',
                    category: 'صبحانه'
                },
                {
                    imagePath: '/assets/images/card/dessert.jpg',
                    title: 'سالمون',
                    category: 'شام'
                },
                {
                    imagePath: '/assets/images/card/salad.jpg',
                    title: 'سالاد',
                    category: 'پیش غذا'
                },
            ] as CardData[]
        }
    }
});
</script>



<template>
    <div class="section-container wsm:flex-col gap-x-10 relative items-center">
        <div class="flex w-full wsm:justify-center">
            <img src="/public/assets/images/about-us.png" class="w-[80%]" alt="">
        </div>
        <div class="flex flex-col w-full">

            <SectionIntro title="درباره ما" />

            <h2 class="aboutus-title">
                بهترین پیشنهاد غذا <br>
                مناسب برای سلامتی شما
            </h2>
            <p class="text">
                فودی به عنوان یک اپلیکیشن هوشمند، با توجه به سلیقه شما و مواد غذایی موجود در آشپزخانه، به شما دستور پخت
                کامل و دقیق ارائه می‌دهد. این دستورات شامل مراحل تهیه غذا، مواد لازم و نحوه آماده‌سازی آن‌ها می‌باشد.
            </p>
            <div class="grid grid-cols-3 gap-x-3 mt-5">
                <div v-for="attr in cardData ">
                    <AboutUsCard :title="attr.title" :category="attr.category" :imagePath="attr.imagePath" />
                </div>
            </div>
        </div>
    </div>
</template>
