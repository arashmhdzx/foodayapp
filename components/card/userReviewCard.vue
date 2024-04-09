<template>
    <div class="flex flex-col relative bg-[#F0F3F3]  text-[#021739] rounded-2xl px-5 pb-3">
        <img :src="imagePath" class=" rounded-full h-[50px] w-[50px] absolute top-[-25px]" alt="">
        <p class=" font pt-10 pb-1 wsm:text-sm">{{ review }}</p>
        <p class="text-lg  font-semibold pt-4">{{ name }}</p>
    </div>
</template>

<script setup>
const { review, name, imagePath } = defineProps({
    review: { type: String, required: true },
    name: { type: String, required: true },
    imagePath: { type: String, required: true },
})
</script>