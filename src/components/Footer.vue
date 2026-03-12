<script setup lang="ts">
import FooterContent from './FooterContent.vue';
import FooterCopyRights from './FooterCopyRights.vue';

</script>

<template>
      <div class="container">
        <FooterContent/>
        <FooterCopyRights />
      </div>
</template>

<style scoped>

footer p {
  font-family: Montserrat Alternates;
  font-weight: 400;
  font-size: 16px;
  line-height: 27.2px;
  letter-spacing: -0.31px;
  color: var(--white-muted);
}

footer a {
  color: var(--white-muted);
  gap: 2rem;
}
footer {
  justify-content: space-evenly;
  border-top: 1px solid var(--divider);
  padding-top: 30px;
}
footer .container {
  display: flex;
  flex-direction: column;
}

</style>