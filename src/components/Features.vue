<template>
    <section class="features">
        <div class="container">
            <section class="section-header">
                <h1>Featured Classes</h1>
                <p>Learn from the world's best</p>
            </section>
            <section class="cards">
                <div class="card">
                    <div>
                        <img src="../assets/Image (Mindset Mastery for Success).png" alt="Mindset Mastery for Success" />
                    </div>
                    <div>
                        <h3>Mindset Mastery for Success</h3>
                        <p>Marcus Johnson</p>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <img src="../assets/Image (Total Body Transformation).png" alt="Total Body Transformation" />
                    </div>
                    <div>
                        <h3>Total Body Transformation</h3>
                        <p>Marcus Johnson</p>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <img src="../assets/Image (Building a Creative Business).png" alt="Building a Creative Business" />
                    </div>

                    <div>
                        <h3>Building a Creative Business</h3>
                        <p>Sophia Williams</p>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <img src="../assets/Image (Product Innovation & Strategy).png"
                            alt="Product Innovation & Strategy" />
                    </div>
                    <div>
                        <h3>Product Innovation & Strategy</h3>
                        <p>David Park</p>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <img src="../assets/Image (Digital Marketing Mastery).png" alt="Digital Marketing Mastery" />
                    </div>
                    <div>
                        <h3>Digital Marketing Mastery</h3>
                        <p>Sarah Mitchell</p>
                    </div>
                </div>
            </section>
        </div>
    </section>
</template>
<style scoped>
.features {
    background-color: var(--bg-dark);
    padding: 5% 0;
}

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

.card img {
    width: 100%;
    height: 350px;
    overflow: hidden;
}

.card,
.instructor-card h3 {
    color: var(--white);
    font-family: Montserrat Alternates;
    letter-spacing: 0.09px;
}

.card p {
    color: var(--accent-dark);
    font-family: Montserrat Alternates;
    font-size: 14px;
    letter-spacing: -0.15px;
}
</style>