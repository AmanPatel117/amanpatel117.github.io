---
title: "GT FSIL — IPO S‑1 NLP"
excerpt: "Regex parsing for 1,000+ S‑1 filings; readability & sentiment analysis to study disclosure quality vs IPO performance."
thumb: /assets/images/headshot.jpg
weight: 4
---
[![View on GitHub](https://img.shields.io/badge/View_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AmanPatel117/Tennis-Analytics-Project)
[![Read the Report](https://img.shields.io/badge/Read_Paper-FF6F61?style=for-the-badge)] (Submitted to KDD 2025, Arxiv paper coming soon!)

# Project Overview
This project develops IPO-Mine, an open-source toolkit and dataset designed to enable large-scale analysis of IPO registration filings. S-1 and F-1 filings submitted to the SEC are extremely long, inconsistently formatted documents that combine narrative disclosures, tables, and embedded visual elements, making them difficult to analyze computationally. IPO-Mine addresses this challenge by building a pipeline that downloads filings from EDGAR, segments them into standardized sections using document structure, and extracts both textual content and embedded images. Using this framework, we constructed a multimodal dataset covering more than 100,000 IPO filings across three decades, allowing researchers to study how companies communicate risks, business strategies, and financial information during the IPO process. The project also introduces benchmarks and exploratory analyses that examine trends in disclosure language, visual communication practices, and the ability of modern multimodal models to interpret financial charts. Together, the toolkit and dataset provide infrastructure for reproducible research on long financial documents and multimodal corporate disclosures.

# My Contributions
My main contribution to the paper was building the parser to parse filings formatted in ASCII, which is the pre-cursor to modern HTML. This was a tough task because unlike HTML, there are no publicly available libraries to help parse text files formatted in ASCII, which led me to have to write parser code from scratch using string operations and regex. The first phase of the work relied on parsing the table of contents from these filings to capture the various sections present in the documents and the page numbers on which they begin. This required the use of regex and software engineering methods to have logical flow between fallback methods to capture as many edge cases as possible.
