<script setup lang="ts">
import { ref } from 'vue'
import { useRoute } from 'vue-router'
import logo from '../assets/Logo.png'

const isOpen = ref(false)
const route = useRoute()

const toggleMenu = () => {
  isOpen.value = !isOpen.value
}

const closeMenu = () => {
  isOpen.value = false
}
</script>

<template>
  <section class="nav-list">
    <router-link to="/" class="logo" @click="closeMenu">
      <img :src="logo" alt="logo" />
    </router-link>

    <button
      class="menu-btn"
      type="button"
      @click="toggleMenu"
      :aria-expanded="isOpen"
      aria-label="Toggle navigation"
    >
      <i class="fa-solid fa-bars"></i>
    </button>

    <ul :class="{ open: isOpen }">
      <li>
        <router-link to="/" @click="closeMenu">الرئيسية</router-link>
      </li>
      <li>
        <router-link to="/categories" @click="closeMenu">الاقسام والمجالات</router-link>
      </li>
      <li>
        <router-link to="/influencers" @click="closeMenu">المؤثرين</router-link>
      </li>
      <li>
        <router-link to="/library" @click="closeMenu">المكتبة</router-link>
      </li>
      <li>
        <router-link to="/about" @click="closeMenu">عن المنصة</router-link>
      </li>
    </ul>
  </section>
</template>

<style scoped>
.nav-list {
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
  gap: 1.5rem;
  position: relative;
}

.logo img {
  height: 50px;
  display: block;
}

.nav-list ul {
  display: flex;
  flex-direction: row-reverse;
  list-style: none;
  gap: 2rem;
}

.nav-list ul li a {
  text-decoration: none;
  color: black;
  font-family: "Almarai", sans-serif;
  font-weight: 700;
  transition: 0.3s ease;
}

.nav-list ul li a:hover {
  color: var(--accent);
}

.router-link-exact-active {
  color: var(--accent);
}

.menu-btn {
  display: none;
  background: none;
  border: none;
  font-size: 22px;
  cursor: pointer;
}


@media (max-width: 768px) {
  .menu-btn {
    display: block;
  }

  .nav-list ul {
    position: absolute;
    top: 70px;
    right: 0;
    width: 220px;
    background: var(--white);
    flex-direction: column;
    gap: 1rem;
    padding: 20px;
    border-radius: 12px;
    display: none;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
    animation: fadeIn 0.2s ease;
  }

  .nav-list ul.open {
    display: flex;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(-5px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>