
---
layout: single
classes: wide
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: 0.0
  caption:
excerpt: >
  Greetings! I’m currently pursuing my Master’s in Analytics at Georgia Tech (’26). I love building
  practical data products—NLP, recommender systems, and GenAI—so teams can make faster, better decisions.

cta_label: "See My Resume"
cta_url: "/assets/docs/Aman_Patel_resume.pdf"
---

## Latest works

{% include feature_row id="portfolio-cards" %}

{% assign features = site.projects | sort: 'weight' %}
{% capture features_markdown %}
{% for p in features %}
- image_path: {{ p.thumb | default: '/assets/images/headshot.jpg' }}
  title: {{ p.title }}
  excerpt: {{ p.excerpt }}
  url: {{ p.url }}
  btn_label: "View Project"
  btn_class: "btn--primary"
{% endfor %}
{% endcapture %}
{% assign feature_row_portfolio-cards = features_markdown | split: '\n' %}
