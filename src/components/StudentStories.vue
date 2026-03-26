<script setup>
import { ref } from 'vue'

const stories = ref([
  {
    quote: "The digital marketing course completely transformed how I approach my campaigns. Within 3 months, we saw a 250% increase in engagement. Sarah's teaching style is incredibly practical and results-driven.",
    author: 'Jennifer Martinez',
    role: 'Marketing Director',
    course: 'Digital Marketing Mastery',
    image: '../assets/Image (Jennifer Martinez).png'
  },
  {
    quote: "The coding bootcamp not only taught me essential programming languages but also the fundamentals of software development. My team completed our app project ahead of schedule, increasing our",
    author: 'David Kim',
    role: 'Software Engineer',
    course: 'Code Academy',
    image: '../assets/Image (David Kim).png'
  },
  {
    quote: "Participating in the UX design seminar enhanced my skills significantly. I implemented user feedback processes and improved our product's usability, resulting in a 40% rise in user satisfaction. The insights were game-changing!",
    author: 'Alice Chen',
    role: 'Product Manager',
    course: 'UX Design Institute',
    image: '../assets/Image (Alice Chen).png'
  },
  {
    quote: "This graphic design workshop opened my eyes to new creative techniques. I was able to redesign our branding in just a week, leading to a 60% boost in customer feedback. The hands-on approach was invaluable.",
    author: 'Michael Thompson',
    role: 'Creative Lead',
    course: 'Visual Arts Academy',
    image: '../assets/Image (Michael Thompson).png'
  }
])

const stars = ref([1,2,3,4,5])
</script>

<template>
  <section class="student-stories">
    <div class="container">
      <header class="student-stories-header">
        <h1>Student Stories</h1>
        <p>Real results from real students</p>
      </header>

      <section class="stories">
        <article v-for="(story, index) in stories" :key="index" class="story">
          <div class="stars">
            <i v-for="star in stars" :key="star" class="fa-solid fa-star"></i>
          </div>

          <blockquote>{{ story.quote }}</blockquote>

          <div class="author">
            <img :src="story.image" :alt="story.author" />
            <div>
              <p>{{ story.author }}</p>
              <span>{{ story.role }}</span>
            </div>
          </div>

          <p class="course">{{ story.course }}</p>
        </article>
      </section>
    </div>
  </section>
</template>

<style scoped>
.student-stories {
  margin-top: 150px;
}

.student-stories-header h1 {
  font-family: Montserrat Alternates;
  font-weight: 700;
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

.stories {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  color: var(--white);
}

.story {
  background-color: var(--bg-card);
  border: 1px solid var(--border);
  border-radius: 15px;
  padding: 30px;
  flex: 1 1 250px;
  font-family: Montserrat Alternates;
}

.stars i {
  color: var(--accent);
}

blockquote {
  margin: 15px 0;
  font-family: Montserrat Alternates;
}

.author {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-top: 15px;
}

.author img {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  object-fit: cover;
}

.author span {
  color: var(--text-secondary);
  font-family: Montserrat Alternates;
  font-weight: 400;
  font-size: 14px;
  letter-spacing: -0.15px;
}


.course {
  margin-top: 10px;
  font-weight: 600;
}
</style>