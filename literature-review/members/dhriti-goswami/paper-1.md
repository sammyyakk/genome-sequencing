# 📄 Paper 1: Deep learning: new computational modelling techniques for genomics
*   **Journal / Conference**: Nature Reviews Genetics (2019)
*   **DOI**: `10.1038/s41576-019-0122-6`
*   **Link**: [Nature Reviews Genetics](https://www.nature.com/articles/s41576-019-0122-6)

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | Genomics data is too large and complex to be mined solely by visual investigation. This paper describes Deep learning modelling techniques and their existing genomic applications. It revolves around 4 major classes of neural networks (Convolutional, Recurrent, Graph Convolutional, fully connected) for supervised ML and explains how they can be used to abstract patterns. |
| **Methodology & Approach** <br>*(2-3 lines)* | This paper is a review of existing methods in this field. Firstly, they group neural networks into four classes- fully connected, convolutional, recurrent and graph convolutional, based on how parameters are shared. Secondly, they explain each class using genomics examples like splice site classification. Lastly, they move from supervised to multimodal to transfer learning to unsupervised methods, citing real models like DeepBind, DeepSEA and Basset as illustration throughout. |
| **Key Results & Findings** <br>*(2-3 lines)* | CNN based models like DeepBind, DeepSEA and Basset performed better than k-mer based and non-deep methods on tasks like DNA accessibility prediction. Secondly, dilated convolutions in Basenji increased the receptive field up to 32kb which allowed long range regulatory dependencies to be captured. Further, the approach of “end to end learning models” in which multiple preprocessing steps are integrated in single model increases its predictive power by removing manual feature engineering. Lastly, unsupervised deep learning techniques help to characterise datasets and the usage of Autoencoders as dimensionality reduction method which improves clustering and visualization of single-cell RNA-seq data. |
| **Limitations Identified** <br>*(1-2 lines)* | Limitations include- not highlighting interpretable relationships in data. Parameters are difficult to interpret due to redundancy and non- linear relationship with output. Data privacy is also an issue along with prediction of casual effects. |
| **Future Scope** <br>*(2-3 lines)* | Future work should focus on enhancing the end-to-end learning approach including the protein structure prediction. Secondly, the ability of deep learning models to deal with multimodal data effectively like analysing gene expression jointly with cell morphology as well as its position in the tissue and in order to protect data, Federated learning approach can be used. |
| **Project Relevance** <br>*(1-2 lines)* | The review is highly relevant to our project as CNN based variant effect models like DeepSEA and Basenji are directly relevant to Variant Prioritization since they predict impact of non-coding variants on chromatin features and gene expression and the discussion on parameter sharing across fully connected vs convolutional layers gives useful background for making design choices in Memory-Efficient Assembly. |
