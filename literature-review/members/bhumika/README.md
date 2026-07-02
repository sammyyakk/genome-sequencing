# 🧑‍🔬 Research Review Dossier: Bhumika
*   **Role**: Research Member
*   **Repository Component**: Literature Review (9 Papers)

This directory houses the systematic literature reviews for Bhumika. Follow the links below to view or edit the respective paper reviews.

---

## 🔬 Section 1: Assigned Papers (Shared Reviews)

1.  **[Paper 1: Deep learning: new computational modelling techniques for genomics](paper-1.md)**
    *   *Nature Reviews Genetics (2019)* | DOI: `10.1038/s41576-019-0122-6`
2.  **[Paper 2: A universal SNP and small-indel variant caller using deep neural networks](paper-2.md)**
    *   *Nature Biotechnology (2018)* | DOI: `10.1038/nbt.4235`
3.  **[Paper 3: An integrated encyclopedia of DNA elements in the human genome](paper-3.md)**
    *   *Nature (2012)* | DOI: `10.1038/nature11247`
4.  **[Paper 4: Cell2location maps fine-grained cell types in spatial transcriptomics](paper-4.md)**
    *   *Nature Biotechnology (2022)* | DOI: `10.1038/s41587-021-01139-4`

---

## 🔬 Section 2: Self-Selected Papers

5.  **[Paper 5: Best Practices for Variant Calling in Clinical Sequencing](paper-5.md)**
    *   *Genome Medicine (2020)* | DOI: `10.1186/s13073-020-00791-w`
6.  **[Paper 6: Whole-Genome Sequencing Surveillance and Machine Learning for Healthcare Outbreak Detection and Investigation: A Systematic Review and Summary](paper-6.md)**
    *   *Antimicrobial Stewardship & Healthcare Epidemiology (2022)* | DOI: `10.1017/ash.2021.241`
7.  **[Paper 7: Comparison of Three Variant Callers for Human Whole Genome Sequencing](paper-7.md)**
    *   *Scientific Reports (2018))* | DOI: `10.1038/s41598-018-36177-7`
8.  **[Paper 8: Machine Learning Enables Detection of Early-Stage Colorectal Cancer by Whole-Genome Sequencing of Plasma Cell-Free DNA](paper-8.md)**
    *   *BMC Cancer (2019)* | DOI: `10.1186/s12885-019-6003-8`
9.  **[Paper 9: Prediction of Antimicrobial Resistance Based on Whole-Genome Sequencing and Machine Learning](paper-9.md)**
    *   *Bioinformatics (2022)* | DOI: `10.1093/bioinformatics/btab681`

---

## 🏁 Section 3: Synthesis Summary

*Leave this section blank until all reviews are complete. Compile these final conclusions to summarize your findings in this folder.*

### 🔍 Common Themes Across Reviewed Papers
*   *Theme 1: [Accuracy of variant calling depends heavily on tool choice and depth so no single tool is perfect, and combining multiple tools (or using AI-based ones like DeepVariant) consistently improves results across nearly all papers reviewed.]*
*   *Theme 2: [Combining multiple orthogonal data sources such as genomic data with electronic health records, single-cell with spatial datan, or DNA with epigenetic marks consistently improves accuracy over using any single data type alone.]*

### 🛠️ Key Methods/Tools That Appear Repeatedly
*   *Method/Tool 1: [GATK (HaplotypeCaller) used as the "gold standard" baseline variant caller across multiple papers for comparison against newer methods.]*
*   *Method/Tool 2: [Convolutional Neural Networks (CNNs) used repeatedly for sequence-based prediction tasks, including DeepVariant , AMR prediction , and general genomics deep learning applications.]*

### 🕳️ Gaps in Literature Relevant to Our Project
*   *Gap 1: [Most studies (e.g., outbreak detection, Paper 6) are retrospective rather than real-time, limiting practical clinical impact so real-time genome sequencing pipelines remain underexplored.]*
*   *Gap 2: [Structural variant (SV) detection remains far less accurate (F1 ~0.80–0.90) than SNV/indel detection (F1 ~0.98–0.99) across all variant-calling papers, showing a clear technical gap our project should be aware of when choosing tools.]*
