<!-- CODE REVIEW: Navbar.vue (Junior Developer)
  Vue Best Practices:
  - CSS: !important is a code smell - increase specificity (nav.navbar) or check what overrides it
  - Good: Composing NavList + Login - each handles its own concern
  - Semantic: Wrap in <header> - <header><nav>...</nav></header> for page structure
  - Consider :class binding for sticky/fixed nav on scroll - common UX pattern
  - Empty line before </script> can be removed - minor style preference
-->
<script setup lang="ts">
import Login from './Login.vue';
import NavList from './NavList.vue';

</script>

<template>
    <nav>
        <div class="container">
            <NavList />
            <Login />
        </div>
    </nav>
</template>
<style scoped>
nav {
    background-color: var(--white) !important;
}

nav .container {
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
}
</style>