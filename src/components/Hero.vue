<!-- CODE REVIEW: Hero.vue (Junior Developer)
  Vue Best Practices:
  - Navigation: Use <router-link> or @click with router.push() for Explore - enables SPA routing
  - Assets: Prefer import img from '@/assets/...' or define in script - enables bundler optimization
  - Good: Alt text on all images - required for accessibility (WCAG)
  - Consider adding loading="lazy" on below-fold images for performance
-->
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
                    <img src="../assets/Carousel_Kim_Kardashian.jpg.png" alt="kim kardashian" />

                    <img src="../assets/Carousel_Joanna_Gaines_4.jpg.png" alt="joanna gaines" />
                </div>
                <div class="col2">
                    <img src="../assets/Carousel_Jeffrey_Pfeffer_CM_NY.jpg.png" alt="jeffrey pfeffer" />
                    <img src="../assets/Carousel_Ryan_Holiday.jpg.png" alt="ryan holiday" />
                    <img src="../assets/Carousel_Ramit_Sethi.jpg.png" alt="ramit sethi" />
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
    flex-wrap: wrap;
    align-items: center;
    gap: 2rem;
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

.intro .intro-artical {
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-style: Regular;
    font-size: 24px;
    line-height: 33.6px;
    letter-spacing: 0.07px;
    color: var(--white);
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

.images {
    display: flex;
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
</style>