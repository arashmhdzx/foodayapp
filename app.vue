<script setup lang="ts">
import Hero from './components/layouts/hero/hero.vue';
import NavBar from './components/layouts/navbar/Navbar.vue'
import AboutUs from './components/layouts/about-us/aboutUs.vue'
import DownlaodSection from './components/layouts/downlaod/download.vue'
import Comments from './components/layouts/comments/comments.vue'
import Footer from './components/layouts/footer/footer.vue'



useHead({
    title: 'فودی | اپلیکیشن سفارش غذا'
});
</script>

<template>
    <NavBar />
    <Hero />
    <AboutUs />
    <DownlaodSection />
    <Comments />
    <Footer />
</template>
