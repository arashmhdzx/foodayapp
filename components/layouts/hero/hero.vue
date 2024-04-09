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
    <div class="hero section-container relative top-[-112px]">
        <div class="hero-bg absolute inset-0"></div>
        <div class="flex flex-col z-10 relative">
            <SectionIntro title="فردا ناهار چی میخوای بپزی؟" />
            <h1 class=" text-7xl text-white my-9 font-bold leading-[80px]">
                پیشنهاد غذا <br>
                برای ناهار بعدیت
            </h1>
            <p class="text-lg text-[#9FACA3]">
                پلیکیشن فودی: راه حلی هوشمند برای انتخاب غذا. <br>
                منوهای متنوع و ایده‌های خلاقانه برای آشپزی. <br>
                با لذت از غذاهای خوشمزه و تنوع غذایی بهتر
            </p>
            <div class="flex">
                <DownloadButton />
            </div>
        </div>
        <div class="flex relative left-[-140px] top-[-50px]">
            <img src="/public/assets/images/hero-mobiles.png" class="w-[600px]" alt="">
        </div>
    </div>
    
</template>
