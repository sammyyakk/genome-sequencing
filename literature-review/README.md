# 📚 Literature Review Guide

This guide details the methodology, search strategies, selection criteria, reading habits, and deadlines for conducting our systematic literature reviews.

---

## 🔍 How to Find Papers (Free)

Accessing scientific literature is critical to building a robust foundation for our models. Use the following portals and strategies to acquire scientific articles without paywalls:

### 🌐 Free Literature Databases & Portals
*   **Google Scholar** ([scholar.google.com](https://scholar.google.com)): The most comprehensive academic search engine. Setup library links to access university or pre-print PDF links.
*   **Semantic Scholar** ([semanticscholar.org](https://www.semanticscholar.org)): AI-powered search engine that highlights key results, citations, and influential references.
*   **PubMed** ([pubmed.ncbi.nlm.nih.gov](https://pubmed.ncbi.nlm.nih.gov)): Essential for biomedical research, clinical trials, and clinical genomic variant analyses.
*   **Sci-Hub**: For paywalled articles, paste the Digital Object Identifier (DOI) or URL into the search bar to access full text instantly.
*   **ResearchGate**: If an article is unavailable, check the authors' profiles. You can directly request a private copy of the paper, which authors are legally allowed to share.
*   **Unpaywall**: A browser extension that automatically searches for legally uploaded, open-access PDF copies of paywalled articles as you browse.
*   **arXiv & bioRxiv**: Always check pre-print servers for the latest pre-publication drafts of genomic papers.

### 🔑 Suggested Search Queries
When searching, combine biology domain terms with machine learning keywords. Recommended search strings:
*   `"genome assembly" AND ("deep learning" OR "graph neural network" OR "GNN")`
*   `"variant prioritization" AND ("machine learning" OR "AI" OR "pathogenicity prediction")`
*   `"long read sequencing" AND "machine learning" AND ("PacBio" OR "Nanopore")`
*   `"whole genome sequencing" AND "clinical AI" AND "decision support"`
*   `"AlphaMissense" OR "ESM1b" OR "Enformer" AND "clinical genetics"`

---

## 🎯 How to Pick Papers

Each member must select and review **5 self-selected papers** alongside the **4 assigned papers** (totaling 9 papers per person). Use these standards to select papers:

*   **Recency**: Published **after 2018** preferably, to capture modern deep learning architectures (Transformers, GNNs, diffusion models).
*   **Relevance**: The paper must directly impact **Problem 3 (Variant Prioritization)** or **Problem 4 (Genome Assembly)**.
*   **Impact Factor & Citation Metrics**: 100+ citations are preferred, though exceptions can be made for highly impactful 2023–2025 papers.
*   **Lock-in Policy**: Post the titles of your selected papers in the group chat before writing them into your file. It operates on a *first-come, first-served* basis to prevent overlapping reviews.

---

## 📖 How to Read a Paper (Efficiently)

Do not read academic papers chronologically from page 1 to the end. It is highly inefficient. Instead, use the **Structural Reading Strategy**:

1.  **Title & Abstract (100% reading)**: Is this relevant to our problems? Does it solve a similar task? If yes, proceed; if no, skip the paper.
2.  **Introduction (Last 2 Paragraphs)**: Read these specifically. This is where authors state their exact contribution, what novel method they built, and the exact biological/ML gaps they are filling.
3.  **Figures & Tables**: Look at the main architecture diagrams and performance figures. A well-designed paper should explain its core methodology visually in 1 or 2 figures.
4.  **Results & Comparative Tables**: What are the actual numbers? How does their model compare with traditional baselines (e.g., F1-score, memory usage, contiguity)?
5.  **Discussion & Conclusion**: What do the authors claim their results mean? What are the clinical or biological implications?
6.  **Methods**: Read this section **only** if you need to replicate their architecture, understand their custom loss function, or inspect their training hyper-parameters.

> [!NOTE]
> **Key Focus Areas**
> You do not need to understand every mathematical derivation or formula. Focus on answering four questions:
> 1. *What biological problem are they trying to solve?*
> 2. *What is their machine learning or algorithmic approach?*
> 3. *What are the key results and performance benefits?*
> 4. *What are the limitations of their work (e.g., memory overhead, error rates)?*

---

## 📅 Milestones & Deadlines

We have strict deadlines to ensure our literature phase is concluded before major model development begins:

*   **📅 June 1, 2025**: All 5 self-selected papers must be claimed, approved by the Team Lead, and metadata pre-filled in your dossier.
*   **📅 June 30, 2025**: All 9 reviews (4 assigned + 5 self-selected) must be completed inside your dedicated review files (`paper-1.md` through `paper-9.md` in your member subdirectory) and submitted via Pull Request.
