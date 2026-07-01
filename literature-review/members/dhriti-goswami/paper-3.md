# 📄 Paper 3: An integrated encyclopedia of DNA elements in the human genome
*   **Journal / Conference**: Nature (2012)
*   **DOI**: `10.1038/nature11247`
*   **Link**: [Nature](https://www.nature.com/articles/nature11247)

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | _The function of vast majority of human genome outside of the well -studied protein region is unknown. This paper has systematically mapped regions of transcription, transcription factor binding, chromatin structure, and histone modification across the genome to assign biochemical function to non-coding regions. |
| **Methodology & Approach** <br>*(2-3 lines)* | The authors generated 1,640 data sets across 147 cell types using assays like ChIP-seq, DNase-seq, RNA-seq, FAIRE-seq and RRBS, standardized across labs with the IDR (irreproducible discovery rate) measure for reproducibility. They then integrated results using discriminative training and unsupervised segmentation methods (ChromHMM, Segway, self-organizing maps) to classify the genome into functional chromatin states. |
| **Key Results & Findings** <br>*(2-3 lines)* |80.4% of the genome showed some biochemical activity (RNA or chromatin related), much more than the 1.2% covered by protein-coding exons. The project identified around 4 lakh enhancer-like and 70 thousand promoter-like regions using chromatin state analysis. It also showed that histone marks and TF binding together could predict most of the variation in RNA expression.  |
| **Limitations Identified** <br>*(1-2 lines)* |The 80.4% figure includes a broad range of evidence types with very different functional confidence, and biochemical activity does not necessarily imply organism-level function. The project also sampled only 119 of approx 1,800 known transcription factors and 13 of 60+ known histone modifications, so the actual extent of functional coverage is not estimated. |
| **Future Scope** <br>*(2-3 lines)* | Future Scope includes expanding data collection to more transcription factors, histone modifications and cell types. It also highlights the goal of eventually assigning every genomic variant a predicted functional impact by combining ENCODE annotations with individual genome sequencing data. |
| **Project Relevance** <br>*(1-2 lines)* | It is relevant to the variant prioritisation pillar of our project as ENCODE annotations like DHSs, TF binding sites and chromatin states are commonly used as features to tell whether a non-coding variant functional or not.   |
