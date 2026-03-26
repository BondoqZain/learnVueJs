<script setup lang="ts">
import { defineAsyncComponent } from 'vue';

const Navbar=defineAsyncComponent(() => import('./components/Navbar.vue'));
const Hero=defineAsyncComponent(() => import('./components/Hero.vue'));
const Features=defineAsyncComponent(() => import('./components/Features.vue'));
const Instructors=defineAsyncComponent(() => import('./components/Instructors.vue'));
const Vision=defineAsyncComponent(() => import('./components/Vision.vue'));
const Statistics=defineAsyncComponent(() => import('./components/Statistics.vue'));
const Mission=defineAsyncComponent(() => import('./components/Mission.vue'));
const StudentStories=defineAsyncComponent(() => import('./components/StudentStories.vue'));
const Faq=defineAsyncComponent(() => import('./components/Faq.vue'));
const MainFooter=defineAsyncComponent(() => import('./components/MainFooter.vue'));
</script>

<template>
  <main>
    <Navbar />
    <Hero />
    <Features />
    <Instructors />
    <Vision />
    <Statistics />
    <Mission />
    <StudentStories />
    <Faq /> 
    <MainFooter />
  </main>
</template>

