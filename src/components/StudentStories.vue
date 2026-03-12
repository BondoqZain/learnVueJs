<template>
    <section class="student-stories">
        <div class="container">
            <section class="student-stories-header">
                <h1>Student Stories</h1>
                <p>Real results from real students</p>
            </section>

            <section class="stories">
                <div class="story">
                    <div class="stars">
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i>
                    </div>
                    <div>
                        <p>
                            "The digital marketing course completely transformed how I
                            approach my campaigns. Within 3 months, we saw a 250% increase
                            in engagement. Sarah's teaching style is incredibly practical
                            and results-driven."
                        </p>
                    </div>
                    <div class="author">
                        <div>
                            <img src="../assets/Image (Jennifer Martinez).png" alt="Jennifer Martinez" />
                        </div>
                        <div>
                            <div>
                                <p>Jennifer Martinez</p>
                            </div>
                            <div><span>Marketing Director</span></div>
                        </div>
                    </div>
                    <div>
                        <p>Digital Marketing Mastery</p>
                    </div>
                </div>

                <div class="story">
                    <div class="stars">
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i>
                    </div>
                    <div>
                        <p>
                            "The coding bootcamp not only taught me essential programming
                            languages but also the fundamentals of software development.
                            My team completed our app project ahead of schedule,
                            increasing our
                        </p>
                    </div>
                    <div class="author">
                        <div>
                            <img src="../assets/Image (Jennifer Martinez).png" alt="David Kim" />
                        </div>
                        <div>
                            <div>
                                <p>David Kim</p>
                            </div>
                            <div><span>Software Engineer</span></div>
                        </div>
                    </div>
                    <div>
                        <p>Code Academy</p>
                    </div>
                </div>

                <div class="story">
                    <div class="stars">
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i>
                    </div>
                    <div>
                        <p>
                            "Participating in the UX design seminar enhanced my skills
                            significantly. I implemented user feedback processes and
                            improved our product's usability, resulting in a 40% rise in
                            user satisfaction. The insights were game-changing!"
                        </p>
                    </div>
                    <div class="author">
                        <div>
                            <img src="../assets/Image (Jennifer Martinez).png" alt="Alice Chen" />
                        </div>
                        <div>
                            <div>
                                <p>Alice Chen</p>
                            </div>
                            <div><span>Product Manager</span></div>
                        </div>
                    </div>
                    <div>
                        <p>UX Design Institute</p>
                    </div>
                </div>

                <div class="story">
                    <div class="stars">
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i
                            class="fa-solid fa-star"></i>
                    </div>
                    <div>
                        <p>
                            "This graphic design workshop opened my eyes to new creative
                            techniques. I was able to redesign our branding in just a
                            week, leading to a 60% boost in customer feedback. The
                            hands-on approach was invaluable."
                        </p>
                    </div>
                    <div class="author">
                        <div>
                            <img src="../assets/Image (Jennifer Martinez).png" alt="Michael Thompson" />
                        </div>
                        <div>
                            <div>
                                <p>Michael Thompson</p>
                            </div>
                            <div><span>Creative Lead</span></div>
                        </div>
                    </div>
                    <div>
                        <p>Visual Arts Academy</p>
                    </div>
                </div>
            </section>
        </div>
    </section>
</template>
<style scoped>
.student-stories{
    margin-top: 150px;
}
.stories {
    color: var(--white);
    display: flex;
    flex-wrap: wrap;
}

.student-stories-header h1 {
    font-family: Montserrat Alternates;
    font-weight: 700;
    font-style: Bold;
    font-size: 72px;
    line-height: 72px;
    letter-spacing: -1.68px;
    color: var(--white);
}

.student-stories-header p {
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-size: 20px;
    line-height: 28px;
    color: var(--text-secondary);
}

.story {
    background-color: var(--bg-card);
    border: 1px solid var(--border);
    border-radius: 15px;
    margin: 10px;
    padding: 30px;
    flex: 1 1 250px;
    font-family: Montserrat Alternates;
}

.stars i {
    color: var(--accent);
}

.author {
    display: flex;
    align-items: center;
    gap: 1rem;
}

.author img {
    justify-items: center;
}

.author span {
    color: var(--text-secondary);
    font-family: Montserrat Alternates;
    font-weight: 400;
    font-size: 14px;
    letter-spacing: -0.15px;
}
</style>