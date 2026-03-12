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