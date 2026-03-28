<script setup lang="ts">
import kimImg from '@/assets/Carousel_Kim_Kardashian.jpg.png'
import joannaImg from '@/assets/Carousel_Joanna_Gaines_4.jpg.png'
import jeffreyImg from '@/assets/Carousel_Jeffrey_Pfeffer_CM_NY.jpg.png'
import ryanImg from '@/assets/Carousel_Ryan_Holiday.jpg.png'
import ramitImg from '@/assets/Carousel_Ramit_Sethi.jpg.png'    

</script>
<template>
    <section class="hero">
        <div class="container">
            <section class="intro">
                <h1 class="orange-big-text">
                    Learn from <br />
                    the best,<br />
                    be your<br />
                    best
                </h1>
                <article class="intro-artical">
                    Forbes 30 Under 30, helping brands scale to 7-figure <br />
                    revenues through data-driven marketing strategies.
                </article>
                <button class="explore">Explore</button>
            </section>
            <section class="images">
                <div class="col1">
                    <img :src="kimImg" alt="Kim Kardashian" loading="lazy"/>

                    <img :src="joannaImg" alt="Joanna Gaines" />
                </div>
                <div class="col2">
                    <img :src="jeffreyImg" alt="Jeffry Pfeffer" />
                    <img :src="ryanImg" alt="Ryan Holidy" />
                    <img :src="ramitImg" alt="Ramit Sethi" />
                </div>
            </section>
        </div>
    </section>

</template>
<style scoped>
.hero {
    display: flex;
    padding: 0 15px;
    justify-content: space-between;
}

.hero .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 3rem;
    max-width: 1200px;
    margin: auto;
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

.intro {
    flex: 1;
    min-width: 300px;
}

.intro .intro-artical {
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-style: Regular;
    font-size: 24px;
    line-height: 30.6px;
    letter-spacing: 0.07px;
    color: var(--white);
    max-width: 500px;

}

.intro .explore {
    border-radius: 48px;
    color: #000;
    border: none;
    background-color: var(--white);
    padding: 15px;
    margin: 20px 0;
    font-family: Montserrat Alternates;
}

.explore:hover {
    transform: translateY(-3px);
}

.images {
    display: flex;
    justify-content: center;
}

.images img {
    margin: 0 10px 10px 10px;
}

.col1 {
    display: flex;
    flex-direction: column;
}

.col2 {
    display: flex;
    flex-direction: column;
}

@media (max-width: 992px) {
    .hero .container {
        flex-direction: column;
        text-align: center;
    }

    .intro-artical {
        margin-left: auto;
        margin-right: auto;
    }

    .images {
        margin-top: 30px;
    }
}

@media (max-width: 576px) {
    .images {
        flex-direction: column;
        align-items: center;
    }

    .col1,
    .col2 {
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
    }

    .images img {
        max-width: 140px;
        height: 180px;
    }
}
</style>