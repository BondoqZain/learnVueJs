<script setup lang="ts">

const faqItems = [
    {
        question: "How do I access the courses?",
        answer: "To access the courses, you need to create an account and purchase the course."
    },
    {
        question: "What is your refund policy?",
        answer: "We offer a 7-day money-back guarantee. If you're not satisfied with your course, you can request a full refund within 7 days of purchase, provided that less than 30% of the course has been completed."
    },
    {
        question: "Do I get a certificate upon completion?",
        answer: "Yes! Once you successfully complete a course, you will receive a digital certificate that you can download and share on your professional profiles."
    },
    {
        question: "Can I access courses on mobile devices?",
        answer: "Yes, our platform is fully responsive and can be accessed on any device with an internet connection, including smartphones and tablets."
    },
    {
        question: "How long do I have access to a course?",
        answer: "Once you purchase a course, you will have lifetime access to it. You can revisit the course materials and lectures whenever you want, even after completing the course."
    },
    {
        question: "Are there any prerequisites for the courses?",
        answer: "Each course may have its own prerequisites, which will be listed on the course page. Generally, we recommend having a basic understanding of programming concepts for our coding courses, but many courses are designed for beginners with no prior experience."
    },
    {
        question: "Can I interact with the instructors?",
        answer: "Yes, we encourage interaction between students and instructors. You can ask questions and participate in discussions through our platform's community forums or during live Q&A sessions if available."
    },
    {
        question: "Do you offer corporate subscriptions?",
        answer: "Yes, we offer corporate subscriptions that provide access to our entire course library for businesses and organizations. This allows companies to provide their employees with access to our courses for professional development and training purposes."

    }
];

</script>


<template>
    <section class="faq">
        <div class="faq-container">
            <h1>FAQ</h1>
            <p class="subtitle">Everything you need to know</p>

            <details v-for="faq in faqItems" class="faq-item">
                <summary>{{ faq.question }}</summary>
                <p>{{ faq.answer }}</p>
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

details[open] summary::after {
    transform: rotate(180deg);
}
</style>
