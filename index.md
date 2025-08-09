---
layout: single
classes: wide
author_profile: true
title: "About Me"

feature_row:
  - image_path: "/assets/images/racquet.jpg"
    title: "Tennis Analytics"
    url: "/projects/tennis-analytics/"
    btn_label: "Details"
    btn_class: "btn--primary"
  - image_path: "/assets/images/ev.webp"
    title: "Deep Learning EV Battery Simulation"
    url: "/projects/unc-rtsg/"
    btn_label: "Details"
    btn_class: "btn--primary"
  - image_path: "/assets/images/runner.webp"
    title: "Injury Prediction for Runners"
    url: "/projects/running/"
    btn_label: "Details"
    btn_class: "btn--primary"
---

<!-- make project card images a consistent size -->
<style>
/* uniform teaser area */
.feature__wrapper .archive__item-teaser {
  height: 180px;          /* tweak to taste (150–220px) */
  overflow: hidden;
  border-radius: 0.5rem;  /* optional: rounded corners */
}
/* scale & crop images to fill */
.feature__wrapper .archive__item-teaser img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}
</style>

<p class="lead">
Hello! I'm a Master's student in Computational Data Science at Georgia Tech with a strong
foundation in mathematics and a passion for building machine learning systems that solve
real-world problems. I have experience working with data and AI across a wide variety of
fields, including finance, sustainability, academia, and tech.<br><br>
My current interests lie at the intersection of data science, applied machine learning, and natural language processing
and LLMs. I'm particularly drawn to:
</p>

<ul>
  <li><strong>Data Science</strong>: data cleaning, feature engineering, data encoding</li>
  <li><strong>Machine Learning</strong>: statistical learning, optimization, deep learning</li>
  <li><strong>LLM Applications</strong>: prompt engineering, Retrieval Augmented Generation, Agentic AI</li>
</ul>

## My Projects

{% include feature_row %}

## Other Interests
I like to spend my free time playing all racquet sports, basketball, volleyball, going to the gym, reading science fiction, and playing video games. I also have been playing piano since I was 5 and recently took a pottery class for the first time, which was an enjoyable experience despite me not being the best at the visual arts.
