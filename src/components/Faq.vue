<!-- CODE REVIEW: Faq.vue (Junior Developer)
  Vue Best Practices:
  - Good: Native <details>/<summary> - accessible, no JS, keyboard-friendly (Vue doesn't over-engineer)
  - Bug: Each <details> has no content - add <p> or <div> inside for the answer text
  - UX: Add [details[open] summary::after { transform: rotate(180deg) } for visual feedback
  - DRY: Consider v-for over faqItems array: [{ question, answer }, ...]
  - Good: Semantic structure - screen readers understand expandable sections
-->
<template>
    <section class="faq">
        <div class="faq-container">
            <h1>FAQ</h1>
            <p class="subtitle">Everything you need to know</p>

            <details class="faq-item">
                <summary>How do I access the courses?</summary>
                <!-- Answer -->
                <p>
                    To access the courses, you need to create an account and purchase the course.
                </p>
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