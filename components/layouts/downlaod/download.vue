<script lang="ts">
import DownloadButton from '../../button/download.vue';

export default defineComponent({
    name: "DownloadSection",
    components: {
        DownloadButton
    },
});
</script>


<template>
    <div class="section-container wsm:px-2 my-20 relative">
        <img src="/public/assets/images/download.png" class="background-image -z-10 w-full wsm:h-[250px]" alt="">
        <div class="download-section-container">
            <h3 class="download-section-title   ">
                میلیون‌ها طعم لذت‌بخش، یک اپلیکیشن رایگان: کلید سرگرمی و سلامتی شما! <br>
                همین حالا دانلود کنید
            </h3>
            <p class="text text-white wsm:text-xs wsm:mt-5">تنها در گوگل پلی قابل دسترسی است</p>
            <DownloadButton />
        </div>
    </div>

</template>
