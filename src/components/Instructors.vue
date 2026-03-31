<script setup lang="ts">
const instructors = [
    {
        name: 'Sarah Mitchell',
        role: 'Digital Marketing Strategist',
        image: new URL('../assets/Image (Sarah Mitchell) (1).png', import.meta.url).href,
        alt: 'Sarah Mitchell'
    },
    {
        name: 'James Rodriguez',
        role: 'Business Leadership Coach',
        image: new URL('../assets/Image (James Rodriguez).png', import.meta.url).href,
        alt: 'James Rodriguez'
    },
    {
        name: 'Elena Chen',
        role: 'Financial Planning Expert',
        image: new URL('../assets/Image (Elena Chen).png', import.meta.url).href,
        alt: 'Elena Chen'
    },
    {
        name: 'Marcus Johnson',
        role: 'Fitness & Wellness Coach',
        image: new URL('../assets/Image (Marcus Johnson).png', import.meta.url).href,
        alt: 'Marcus Johnson'
    },
    {
        name: 'Sophia Williams',
        role: 'Creative Entrepreneur',
        image: new URL('../assets/Image (Sophia Williams).png', import.meta.url).href,
        alt: 'Sophia Williams'
    }
];
</script>


<template>
    <section class="instructors">
        <div class="container">
            <section class="section-header">
                <h1>Instructors</h1>
                <p>Meet the experts who will guide your journey</p>
            </section>
            <section class="cards">
                <div class="instructor-card" v-for="instructor in instructors" :key="instructor.name">
                    <div>
                        <img :src="instructor.image" :alt="instructor.alt" />
                    </div>
                    <div>
                        <h3>{{ instructor.name }}</h3>
                        <p>{{ instructor.role }}</p>
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




.instructors .cards {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
}

.instructor-card {
    margin: 10px;
    flex: 0 0 250px;
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
    height: 250px;
    object-fit: cover;
}

.instructor-card h3 {
    color: var(--white);
    font-family: Montserrat Alternates;
    letter-spacing: 0.09px;
}
</style>Í