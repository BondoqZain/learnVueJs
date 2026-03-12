<script setup lang="ts">
import Login from './Login.vue';
import NavList from './NavList.vue';

</script>

<template>
    <div class="container">
        <nav>
            <NavList />
            <Login />
        </nav>
    </div>  
</template>
<style scoped>
nav {
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
    background-color: var(--white);
}
</style>