<script setup lang="ts">
import FooterContent from './FooterContent.vue';
import FooterCopyRights from './FooterCopyRights.vue';
</script>

<template>
  <footer>
    <div class="container">
      <FooterContent />
      <FooterCopyRights />
    </div>
  </footer>
</template>

<style scoped>

footer {
  justify-content: space-evenly;
  border-top: 1px solid var(--divider);
  padding-top: 30px;
    background: linear-gradient(
    0deg,
    #0e1733 100%,
    rgba(14, 23, 51, 0.4) 40%,
    #0e1733 100%
  );
}

footer .container {
  display: flex;
  flex-direction: column;
}
</style>