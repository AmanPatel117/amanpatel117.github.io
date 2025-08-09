
---
permalink: /portfolio/
layout: single
title: "Latest works"
classes: wide
---

{% include feature_row %}

{% capture feature_row %}
- title: "BlueConduit — GenAI tooling & survival modeling"
  excerpt: "Built LLM scraping + LangChain internal tools that cut data ingestion time 20%+. Led NN approach to predict water main survival times; refactored Databricks deployment with drift monitoring."
  url: "/projects/blueconduit/"
  btn_label: "Details"
  btn_class: "btn--primary"
- title: "State Farm — RAG Q&A and exec analytics"
  excerpt: "RAG pipeline (LlamaIndex) saved 50+ analyst hours on rate filings; SQL for claim payout modeling; Power BI dashboard on state policy → quote conversion."
  url: "/projects/state-farm/"
  btn_label: "Details"
  btn_class: "btn--primary"
- title: "Tremau — Semantic search recommender"
  excerpt: "OpenAI embeddings + Pinecone vector DB to recommend content to moderators; trained NN/GBM classifiers for policy violations (75%+ acc)."
  url: "/projects/tremau/"
  btn_label: "Details"
  btn_class: "btn--primary"
- title: "GT FSIL — IPO S‑1 NLP"
  excerpt: "Regex package parsing 1,000+ S‑1 filings; readability & sentiment analysis to study disclosure quality vs IPO performance."
  url: "/projects/gt-fsil/"
  btn_label: "Details"
  btn_class: "btn--primary"
- title: "UNC Real‑Time Systems — EV battery sim"
  excerpt: "Integrated LSTM driving‑behavior models into 4‑month EV battery simulation; +2% lifespan (~30 days)."
  url: "/projects/unc-rtsg/"
  btn_label: "Details"
  btn_class: "btn--primary"
{% endcapture %}

{% include feature_row %}
