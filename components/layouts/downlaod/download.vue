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
        <div class="flex flex-col items-center justify-between absolute top-0 left-0 w-full h-full pt-20 pb-14 wsm:p-10">
            <h3 class="text-white wsm:text-lg text-4xl text-center font-bold leading-[55px] wsm:leading-normal ">
                میلیون‌ها طعم لذت‌بخش، یک اپلیکیشن رایگان: کلید سرگرمی و سلامتی شما! <br>
                همین حالا دانلود کنید
            </h3>
            <p class="text text-white wsm:text-xs wsm:mt-5">تنها در گوگل پلی قابل دسترسی است</p>
            <DownloadButton />
        </div>
    </div>

</template>
