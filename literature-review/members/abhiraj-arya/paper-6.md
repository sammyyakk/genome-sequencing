# 📄 Paper 6: Deep Learning-Based Identification of Genetic Variants: Application to Alzheimer's Disease Classification
*   **Journal / Conference**: Briefings in Bioinformatics (2022)
*   **DOI**: `10.1093/bib/bbac141`

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | _[Alzheimer's disease is highly heritable (up to 80%), deep learning had rarely been applied to genome-wide association studies (GWAS) due to the high-dimension low-sample-size (HDLSS) problem inherent to genomic data.]_ |


| **Methodology & Approach** <br>*(2-3 lines)* | _[The authors introduced deep learning framework named SWAT-CNN. The genome was first divided into small parts, and a CNN was used to find regions that might be linked to the disease. Then, a Sliding Window Association Test identified important DNA variations , and these were used to train another CNN model to predict the disease, which was then compared with models like Random Forest and XGBoost.]_ |


| **Key Results & Findings** <br>*(2-3 lines)* | _[The SWAT-CNN model successfully found important gene regions linked to the disease, and also discovered some new possible disease-related genes. Using the top 4000 SNPs (Single Nucleotide Polymorphisms), the model achieved 75% accuracy and performed better than Random Forest, XGBoost]_ |


| **Limitations Identified** <br>*(1-2 lines)* | _[As the research used a relatively small sample size (N=981), which limits how broadly the results can be applied to other groups. Also it only performed binary classification and both the CNN and PLINK selected different sets of SNPs making it difficult to understand which genetic changes were truly responsible for disease. ]_ |


| **Future Scope** <br>*(2-3 lines)* | _[Applying SWAT-CNN to larger genome sequencing datasets to discover more SNPs related to Alzheimer's and improve the model's accuracy.They also suggest to expand the framework to earlier disease stages, and replacing binary labels with quantitative endophytes , which could better reflect genetic risk in specefic disease paths. ]_ |


| **Project Relevance** <br>*(1-2 lines)* | _[The research shows that deep learning can support traditional genome-wide association studies by grouping nearby SNPs to find disease-related variants and build effective classification models]_ |
