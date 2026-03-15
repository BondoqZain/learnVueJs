<!-- CODE REVIEW: Mission.vue (Junior Developer)
  Vue Best Practices:
  - Duplicate .mission h2 selector (lines 18 & 34) - merge into one rule to avoid redundancy
  - Same .orange-big-text duplication as Vision.vue - extract to shared styles
  - Good: Clear semantic structure
  - Vision and Mission are very similar - consider a single VisionMission component with a prop
-->
<template>
    <section class="mission">
        <div class="container">
            <h1 class="orange-big-text">Our Mission</h1>
            <h2>
                Democratizing excellence by connecting passionate learners with
                <br />
                industry-leading instructors, fostering a community of continuous
                <br />
                growth and transformation.
            </h2>
        </div>
    </section>
</template>

<style scoped>
.mission h2 {
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-style: Regular;
    font-size: 30px;
    color: var(--white);
    letter-spacing: 0.4px;
    text-align: center;
}

.mission h1 {
    justify-items: center;
    text-align: center;
}

.mission h2 {
    margin-bottom: 0;
}

.orange-big-text {
    font-family: Montserrat Alternates;
    font-weight: 700;
    font-style: Bold;
    font-size: 96px;
    line-height: 91.2px;
    letter-spacing: -2.4px;
    color: var(--accent);
}
</style>