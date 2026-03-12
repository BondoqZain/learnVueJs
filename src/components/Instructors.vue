<template>
    <section class="instructors">
        <div class="container">
            <section class="section-header">
                <h1>Instructors</h1>
                <p>Meet the experts who will guide your journey</p>
            </section>
            <section class="cards">
                <div class="instructor-card">
                    <div>
                        <img src="../assets/Image (Sarah Mitchell) (1).png" alt="Sarah Mitchell" />
                    </div>
                    <div>
                        <h3>Sarah Mitchell</h3>
                        <p>Digital Marketing Strategist</p>
                    </div>
                </div>

                <div class="instructor-card">
                    <div>
                        <img src="../assets/Image (James Rodriguez).png" alt="James Rodriguez" />
                    </div>
                    <div>
                        <h3>James Rodriguez</h3>
                        <p>Business Leadership Coach</p>
                    </div>
                </div>

                <div class="instructor-card">
                    <div>
                        <img src="../assets/Image (Elena Chen).png" alt="Elena Chen" />
                    </div>
                    <div>
                        <h3>Elena Chen</h3>
                        <p>Financial Planning Expert</p>
                    </div>
                </div>

                <div class="instructor-card">
                    <div>
                        <img src="../assets/Image (Marcus Johnson).png" alt="Marcus Johnson" />
                    </div>
                    <div>
                        <h3>Marcus Johnson</h3>
                        <p>Fitness & Wellness Coach</p>
                    </div>
                </div>

                <div class="instructor-card">
                    <div>
                        <img src="../assets/Image (Sophia Williams).png" alt="Sophia Williams" />
                    </div>
                    <div>
                        <h3>Sophia Williams</h3>
                        <p>Creative Entrepreneur</p>
                    </div>
                </div>

                <div class="instructor-card">
                    <div>
                        <img src="../assets/Image (Marcus Johnson).png" alt="Marcus Johnson" />
                    </div>
                    <div>
                        <h3>Marcus Johnson</h3>
                        <p>Fitness & Wellness Coach</p>
                    </div>
                </div>
            </section>
        </div>
    </section>
</template>
<style scoped>
.section-header h1 {
    color: var(--white);
    font-family: Montserrat Alternates;
    font-weight: 700;
    font-style: Bold;
    font-size: 72px;
    line-height: 72px;
    letter-spacing: -1.68px;
}

.section-header p {
    font-family: Montserrat Alternates;
    font-style: Regular;
    line-height: 28px;
    letter-spacing: -0.45px;
    color: var(--white);
}

.cards {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
}

.card {
    margin: 10px;
    flex: 1 1 250px;
}

.instructors .cards {
    justify-content: space-between;
    flex-wrap: wrap;
}

.instructor-card {
    margin: 10px;
    flex: 1 1 200px;
}

.instructor-card p {
    color: var(--text-secondary);
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-size: 14px;
    letter-spacing: -0.15px;
}

.instructor-card img {
    width: 100%;
    overflow: hidden;
}

.instructor-card h3 {
    color: var(--white);
    font-family: Montserrat Alternates;
    letter-spacing: 0.09px;
}
</style>