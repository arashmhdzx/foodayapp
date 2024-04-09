<script lang="ts">
import { defineComponent } from 'vue';
import NavLink from '../../link/NavLink.vue';
import RegisterButton from '../../button/register.vue';

export default defineComponent({
    name: "NavBar",
    components: {
        NavLink,
        RegisterButton,
    },
    data() {
        return {
            isScrolled: false
        };
    },
    mounted() {
        window.addEventListener('scroll', this.handleScroll);
    },
    beforeUnmount() {
        window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
        handleScroll() {
            this.isScrolled = window.scrollY > 0;
        }
    }
});
</script>

<template>
    <nav class="navbar" :class="{ 'active-navbar':isScrolled }">
        <div class="flex items-center">
            <NavLink title="خانه" linkTo="#hero" />
            <NavLink title="درباره ما" linkTo="#about-us" />
            <NavLink title="نظرات" linkTo="#comments" />
            <NavLink title="اپلیکیشن" linkTo="#download" />
        </div>
        <div class="flex rounded-full" :class="{ 'shadow-lg shadow-white':isScrolled }" >
            <RegisterButton />
        </div>
    </nav>
</template>