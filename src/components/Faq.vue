<template>
    <section class="faq">
        <div class="faq-container">
            <h1>FAQ</h1>
            <p class="subtitle">Everything you need to know</p>

            <details class="faq-item">
                <summary>How do I access the courses?</summary>
            </details>

            <details class="faq-item">
                <summary>What is your refund policy?</summary>
            </details>

            <details class="faq-item">
                <summary>Do I get a certificate upon completion?</summary>
            </details>

            <details class="faq-item">
                <summary>Can I access courses on mobile devices?</summary>
            </details>

            <details class="faq-item">
                <summary>How long do I have access to a course?</summary>
            </details>

            <details class="faq-item">
                <summary>Are there any prerequisites for the courses?</summary>
            </details>

            <details class="faq-item">
                <summary>Can I interact with the instructors?</summary>
            </details>

            <details class="faq-item">
                <summary>Do you offer corporate subscriptions?</summary>
            </details>
        </div>
    </section>
</template>

<style scoped>
.faq {
    padding: 80px 20px;
    color: var(--white);
    font-family: Montserrat Alternates;
}

.faq-container {
    max-width: 900px;
    margin: auto;
}

.faq-container h1 {
    font-size: 70px;
    margin-bottom: 10px;
}

.subtitle {
    color: var(--text-subtitle);
    margin-bottom: 50px;
    font-size: 18px;
}

.faq-item {
    border-bottom: 1px solid var(--border-light);
    padding: 20px 0;
}

summary {
    font-size: 20px;
    font-weight: 600;
    list-style: none;
    position: relative;
}

summary::after {
    content: "▾";
    position: absolute;
    right: 0;
    transition: 0.3s;
}
</style>