<!-- CODE REVIEW: App.vue (Junior Developer)
  Vue Best Practices:
  - Import casing: './instructors.vue' should match file name - use PascalCase (Instructors.vue) for consistency
  - Good: <script setup> is the recommended Composition API style - no need for defineComponent
  - Good: Clear component hierarchy - single responsibility per component
  - Accessibility: Add <main> landmark wrapping content, or skip-to-content link for keyboard users
  - Consider lazy-loading below-fold components: defineAsyncComponent for Vision, Statistics, Mission, etc.
  - Empty <style scoped> can be removed - Vue allows omitting unused blocks
-->
<script setup lang="ts">
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Features from './components/Features.vue'; 
import MainFooter from './components/MainFooter.vue';
import Instructors from './components/instructors.vue';
import Vision from './components/Vision.vue';
import Statistics from './components/Statistics.vue';
import Mission from './components/Mission.vue';
import StudentStories from './components/StudentStories.vue';
import Faq from './components/Faq.vue';
</script>

<template>
  <div>
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
  </div>
</template>

<style scoped></style>
