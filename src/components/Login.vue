<!-- CODE REVIEW: Login.vue (Junior Developer)
  Vue Best Practices:
  - Naming: Component does more than login (basket + login) - consider HeaderActions or NavActions
  - Interactivity: Login button has no @click - add handler or wrap in router-link to /login
  - Interactivity: Basket has no @click or href - users cannot access cart
  - Use <button type="button"> explicitly - prevents accidental form submission in nested forms
  - Good: CSS variables (var(--primary)) - excellent for theming and dark mode
  -->
<template>
    <section class="login">
        <div class="basket">
            <i class="fa-solid fa-cart-shopping"></i>
        </div>
        <div>
            <button class="login-btn">تسجيل دخول</button>
        </div>
    </section>
</template>
<style scoped>
.login {
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    gap: 1rem;
}

.login-btn {
    background-color: var(--primary);
    border: none;
    color: var(--white);
    padding: 10px;
    font-family: Almarai;
    line-height: 114.99999999999999%;
    letter-spacing: 0%;
    vertical-align: middle;
    opacity: 1;
    border-radius: 20px;
}

.basket i {
    background-color: var(--primary-light);
    border-radius: 50%;
    padding: 10px;
    color: var(--primary);
}
</style>