<!-- CODE REVIEW: MainFooter.vue (Junior Developer)
  Vue Best Practices:
  - Good: Composition - FooterContent + FooterCopyRights - clear separation of concerns
  - Good: <script setup> with clean imports
  - CSS bug: footer has justify-content but no display: flex - justify-content has no effect
  - Semantic: <footer> is correct - screen readers identify as footer landmark
-->
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