<!-- CODE REVIEW: FooterCopyRights.vue (Junior Developer)
  Vue Best Practices:
  - Good: Single responsibility - does one thing well
  - Dynamic year: Use {{ new Date().getFullYear() }} - no manual updates needed each year
  - Good: &copy; entity for copyright symbol
  - Add <script setup> if using dynamic year - template expressions only
-->
<template>
    <div class="rights">
        <p>&copy;2026 MulhimNas. All rights reserved.</p>
    </div>
</template>

<style scoped>
.rights {
  text-align: center;
  margin-top: 20px;
}
</style>