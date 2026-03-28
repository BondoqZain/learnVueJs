<script setup lang="ts">
const year = new Date().getFullYear();
</script>
<template>
  <div class="rights">
    <p>&copy; {{ year }} MulhimNas. All rights reserved.</p>
  </div>
</template>

<style scoped>
.rights {
  text-align: center;
  margin-top: 20px;
  color: var(--white-muted);
}
</style>