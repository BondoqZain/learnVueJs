<script setup lang="ts">
const featuredClasses = [
    {
        id: 1,
        title: 'Mindset Mastery for Success',
        instructor: 'Marcus Johnson',
        image: new URL('../assets/Image (Mindset Mastery for Success).png', import.meta.url).href,
    },
    {
        id: 2,
        title: 'Total Body Transformation',
        instructor: 'Marcus Johnson',
        image: new URL('../assets/Image (Total Body Transformation).png', import.meta.url).href,
    },
    {
        id: 3,
        title: 'Building a Creative Business',
        instructor: 'Sophia Williams',
        image: new URL('../assets/Image (Building a Creative Business).png', import.meta.url).href,
    },
    {
        id: 4,
        title: 'Product Innovation & Strategy',
        instructor: 'David Park',
        image: new URL('../assets/Image (Product Innovation & Strategy).png', import.meta.url).href,
    },
    {
        id: 5,
        title: 'Digital Marketing Mastery',
        instructor: 'Sarah Mitchell',
        image: new URL('../assets/Image (Digital Marketing Mastery).png', import.meta.url).href,
    },
];

const handleClick = (item: any) => {
    console.log('Clicked:', item.title);
};
</script>

<template>
    <section class="features">
        <div class="container">

            <header class="section-header">
                <h1>Featured Classes</h1>
                <p>Learn from the world's best</p>
            </header>

            <section class="cards">
                <div 
                    class="card" 
                    v-for="item in featuredClasses" 
                    :key="item.id"
                    @click="handleClick(item)"
                >
                    <div>
                        <img :src="item.image" :alt="item.title" />
                    </div>

                    <div>
                        <h3>{{ item.title }}</h3>
                        <p>{{ item.instructor }}</p>
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
    font-size: 72px;
    line-height: 72px;
    letter-spacing: -1.68px;
}

.section-header p {
    font-family: Montserrat Alternates;
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
    flex: 0 0 250px;
    color: var(--white);
    font-family: Montserrat Alternates;
    cursor: pointer;
    transition: 0.3s;
    letter-spacing: 0.09px;
}

.card img {
    width: 100%;
    height: 350px;
    object-fit: cover;
}

.card p {
    color: var(--accent-dark);
    font-size: 14px;
    letter-spacing: -0.15px;
}

.card:hover {
    transform: translateY(-5px);
}
</style>