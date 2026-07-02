# 📄 Paper 5: DeepC: Predicting 3D Genome Folding Using Megabase-Scale Transfer Learning
*   **Journal / Conference**: Nature Methods (2020)
*   **DOI**: `10.1038/s41592-020-0854-y`

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | Earlier 3D genome folding models either captured fine DNA sequence information over small windows or captured large genomic context using coarse features, but not both. DeepC bridges this gap by combining single-nucleotide resolution with megabase-scale context. |
| **Methodology & Approach** <br>*(2-3 lines)* | DeepC uses a two-stage transfer learning framework. First, a convolutional neural network (CNN) is trained to predict 936 chromatin features from DNA sequences using ENCODE and Roadmap datasets. These learned feature representations are then transferred to a second network that predicts Hi-C chromatin contact maps from 1 Mb DNA sequences by dividing them into 200 bins of 5 kb each. To improve learning, the model applies skeleton percentile normalization, which removes genomic distance bias and enables it to focus on biologically meaningful chromatin structures|
| **Key Results & Findings** <br>*(2-3 lines)* | DeepC achieved strong predictive performance across multiple datasets, including Pearson correlations of 0.57 (smoothed) and 0.36 (raw) on the GM12878 cell line, and 0.51 (smoothed) and 0.28 (raw) on the K562 cell line. It generalized to previously unseen chromosomes, outperformed HiC-Reg, learned cell-type-specific folding patterns, and produced reliable predictions even from Hi-C datasets containing approximately 100 million contacts, although 10 million contacts were insufficient for accurate training.|
| **Limitations Identified** <br>*(1-2 lines)* |DeepC accurately predicts TADs but underestimates insulation boundaries and produces smoother CTCF loop signals because chromatin factors such as cohesin are not encoded in the DNA sequence. The model is limited to 1 Mb genomic windows, cannot capture inter-chromosomal or A/B compartment interactions, and generally requires separate models for different cell types.|
| **Future Scope** <br>*(2-3 lines)* | Future versions of DeepC could model larger genomic regions to capture inter-chromosomal interactions and A/B compartments, while incorporating additional biological factors such as cohesin and chromatin proteins to improve loop prediction. The framework could also be extended to predict the effects of disease-associated genetic variants across multiple cell types, supporting precision medicine and functional variant interpretation.|
| **Project Relevance** <br>*(1-2 lines)* | DeepC provides an effective framework for learning biologically meaningful information directly from DNA sequences. Its use of CNNs and transfer learning offers valuable insights for designing deep learning models for genome sequencing and analysis.|
