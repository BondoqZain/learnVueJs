<template>
    <div class="container">
        <section class="statistics">
            <div class="statistics-card">
                <h1>500K+</h1>
                <p>Active Students</p>
            </div>

            <div class="statistics-card">
                <h1>100+</h1>
                <p>Expert Instructors</p>
            </div>

            <div class="statistics-card">
                <h1>180+</h1>
                <p>Classes</p>
            </div>
        </section>
    </div>
</template>

<style scoped>
.statistics {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-evenly;
    color: var(--white);
    text-align: center;
}

.statistics-card {
    flex: 1 1 250px;
}

.statistics-card h1 {
    font-family: Montserrat Alternates;
    font-size: 50px;
    text-align: center;
    margin-bottom: 0;
    margin-top: 0;
}

.statistics-card p {
    font-family: Montserrat Alternates;
}
</style>