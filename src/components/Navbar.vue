<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue'
import Login from './Login.vue'
import NavList from './NavList.vue'

const isSticky = ref(false)

const handleScroll = () => {
  isSticky.value = window.scrollY > 20
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll)
})
</script>

<template>
  <header>
    <nav :class="{ sticky: isSticky }" class="navbar">
      <div class="container">
        <NavList />
        <Login />
      </div>
    </nav>
  </header>
</template>

<style scoped>
.navbar {
  background-color: var(--white);
  padding: 12px 0;
  transition: all 0.3s ease;
}

.navbar.sticky {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
  z-index: 1000;
}

.navbar .container {
  display: flex;
  flex-direction: row-reverse;
  justify-content: space-between;
  align-items: center;
}

@media (max-width: 768px) {
  .navbar .container {
    padding: 0 15px;
  }
}
</style>