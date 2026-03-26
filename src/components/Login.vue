<script setup lang="ts">
import { useRouter } from 'vue-router';

const router = useRouter();

const goToLogin = () => {
  router.push('/login');
};

const goToCart = () => {
  router.push('/cart');
};
</script>

<template>
  <section class="header-actions">
    <button class="basket" type="button" @click="goToCart">
      <i class="fa-solid fa-cart-shopping"></i>
    </button>

    <button class="login-btn" type="button" @click="goToLogin">
      تسجيل دخول
    </button>
  </section>
</template>

<style scoped>
.header-actions {
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
  gap: 1rem;
}

button {
  cursor: pointer;
  border: none;
}

.login-btn {
  background-color: var(--primary);
  color: var(--white);
  padding: 10px 16px;
  font-family: Almarai;
  border-radius: 20px;
  transition: 0.3s ease;
}

.login-btn:hover {
  opacity: 0.85;
}

.basket {
  background-color: var(--primary-light);
  border-radius: 50%;
  padding: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
}

@media (max-width: 768px) {
  .login-btn {
    padding: 8px 12px;
    font-size: 14px;
  }

  .basket {
    padding: 8px;
  }
}

@media (max-width: 480px) {
  .header-actions {
    gap: 0.5rem;
  }

  .login-btn {
    font-size: 13px;
    padding: 6px 10px;
  }

  .basket i {
    font-size: 14px;
  }
}
</style>