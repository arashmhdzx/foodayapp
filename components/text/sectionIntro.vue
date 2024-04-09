<template>
    <div class="flex items-center text-[#ff9123]">
        <span class="border px-3 border-[#ff9123] ml-3"></span>
        <p>{{ title }}</p>
    </div>
</template>

<script setup>
const { title } = defineProps({
    title: { type: String, required: true },
})
</script>