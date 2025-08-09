---
layout: single
classes: wide
author_profile: true
title: ""
excerpt: "Greetings! I'm currently pursuing my Master's in Analytics at Georgia Tech (’26). I love building practical data products—NLP, recommender systems, and GenAI—so teams can make faster, better decisions."
cta_label: "See My Resume"
cta_url: "/assets/docs/Aman_Patel_resume.pdf"
---

## Latest works

{% include feature_row %}
{% capture feature_row %}
- title: "BlueConduit — GenAI tooling & survival modeling"
  excerpt: "LLM scraping + LangChain internal tools; Databricks with drift monitoring; NN survival modeling."
  url: "/projects/blueconduit/"
  btn_label: "Details"
  btn_class: "btn--primary"
- title: "State Farm — RAG Q&A and exec analytics"
  excerpt: "RAG (LlamaIndex) saved 50+ analyst hours; SQL for claim payout; Power BI on policy → conversion."
  url: "/projects/state-farm/"
  btn_label: "Details"
  btn_class: "btn--primary"
- title: "Tremau — Semantic search recommender"
  excerpt: "OpenAI + Pinecone vector search; NN/GBM classification (75%+ acc)."
  url: "/projects/tremau/"
  btn_label: "Details"
  btn_class: "btn--primary"
{% endcapture %}
{% include feature_row %}
