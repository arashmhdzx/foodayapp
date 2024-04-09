<script lang="ts">
import SectionIntro from '../../text/sectionIntro.vue';
import DownloadButton from '../../button/download.vue';

export default defineComponent({
    name: "Hero",
    components: {
        SectionIntro,
        DownloadButton
    },
});
</script>


<template>
    <div class="hero section-container">
        <div class="hero-bg absolute inset-0"></div>
        <div class="flex flex-col z-10 relative wsm:mt-5">
            <SectionIntro title="فردا ناهار چی میخوای بپزی؟" />
            <h1 class="hero-title">
                پیشنهاد غذا <br>
                برای ناهار بعدیت
            </h1>
            <p class="text-lg text-[#9FACA3] wsm:text-sm">
                پلیکیشن فودی: راه حلی هوشمند برای انتخاب غذا. <br>
                منوهای متنوع و ایده‌های خلاقانه برای آشپزی. <br>
                با لذت از غذاهای خوشمزه و تنوع غذایی بهتر
            </p>
            <div class="flex">
                <DownloadButton />
            </div>
        </div>
        <div class="hero-image">
            <img src="/public/assets/images/hero-mobiles.png" class="w-[600px] wsm:w-[350px]" alt="">
        </div>
    </div>
    
</template>
