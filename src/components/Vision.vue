<!-- CODE REVIEW: Vision.vue (Junior Developer)
  Vue Best Practices:
  - Consider adding <script setup> for consistency - even empty components benefit from explicit setup
  - Good: Semantic <section> usage
  - DRY: .orange-big-text is duplicated in Hero.vue, Mission.vue - consider a shared CSS module or global utility class
-->
<template>
    <section class="vision">
        <div class="container">
            <h1 class="orange-big-text">Our Vision</h1>
            <h2>
                To create a world where knowledge knows no boundaries, <br />
                empowering individuals to unlock their full potential through <br />
                accessible, world-class education.
            </h2>
        </div>
    </section>
</template>
<style scoped>
.orange-big-text {
    font-family: Montserrat Alternates;
    font-weight: 700;
    font-style: Bold;
    font-size: 96px;
    line-height: 91.2px;
    letter-spacing: -2.4px;
    color: var(--accent);
}

.vision {
    margin-top: 150px;
}

.vision h2 {
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-style: Regular;
    font-size: 30px;
    color: var(--white);
    letter-spacing: 0.4px;
    text-align: center;
}

.vision h1 {
    justify-items: center;
    text-align: center;
}
</style>