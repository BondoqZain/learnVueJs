<!-- CODE REVIEW: NavList.vue (Junior Developer)
  Vue Best Practices:
  - Use router-link instead of <a href="#"> for SPA navigation - avoids full page reload
  - href="#" causes page jump - use @click.prevent or router-link
  - :active only styles on mousedown - consider :hover for better UX, or router-link-active for current route
  - Good: Responsive design with media query hiding nav on mobile
  - Consider adding a mobile menu toggle (hamburger) since nav hides at 768px - users lose navigation
-->
<template>
    <section class="nav-list">
        <img src="../assets/Logo.png" alt="logo" />
        <ul>
            <li><a href="#">الرئيسية</a></li>
            <li><a href="#">الاقسام والمجالات</a></li>
            <li><a href="#">المؤثرين</a></li>
            <li><a href="#">المكتبة</a></li>
            <li><a href="#">عن المنصة</a></li>
        </ul>
    </section>
</template>
<style scoped>
.nav-list {
    display: flex;
    margin-right: 10px;
    flex-direction: row-reverse;
}

.nav-list img {
    padding: 10px;
}

.nav-list ul {
    display: flex;
    flex-direction: row-reverse;
    list-style: none;
    gap: 2rem;
    margin-right: 10px;
}

.nav-list ul li {
    font-family: "Almarai", sans-serif;
    font-weight: 700;
    font-size: 16px;
    line-height: 24px;
    letter-spacing: 0px;
    text-align: right;
}

.nav-list ul li:active {
    color: var(--accent);
}
@media screen and (max-width: 768px) {
  .nav-list ul {
    display: none;
  }
}
</style>