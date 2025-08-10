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
  - image_path: "/assets/images/restaurant.webp"
    title: "Safe Diner ATL"
    url: "/projects/cx4242/"
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

<style>
.feature__wrapper .archive__item-teaser img {
  max-height: 160px;  /* Change this number for bigger/smaller images */
  width: auto;
  height: auto;
  display: block;
  margin: 0 auto;
}
/* Style for primary buttons */
.btn--primary {
  background: linear-gradient(135deg, #00c6ff, #0072ff); /* teal to blue */
  border: none;
  color: white !important;
  padding: 0.6em 1.2em;
  font-weight: 600;
  border-radius: 6px;
  transition: transform 0.15s ease, box-shadow 0.15s ease;
}

.btn--primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 114, 255, 0.3);
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
