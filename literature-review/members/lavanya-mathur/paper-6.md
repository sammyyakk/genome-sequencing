# 📄 Paper 6: Predicting 3D Genome Folding from DNA Sequence with Akita
*   **Journal / Conference**: Nature Methods (2020)
*   **DOI**: `10.1038/s41592-020-0958-4`

---

## 🔬 Literature Review Table

    | Evaluation Field | Researcher Analysis |
    | :--- | :--- |
    | **Problem Addressed** <br>*(1-2 lines)* |  The 3D folding of DNA inside the nucleus determines gene regulation, but it was unclear whether folding patterns could be predicted directly from DNA sequence alone, without experimental measurement.|
    | **Methodology & Approach** <br>*(2-3 lines)* | The authors built Akita, a convolutional neural network with a "trunk" (extracts sequence features like CTCF motifs) and a "head" (converts features into a 2D contact map). It takes ~1 Mb of DNA sequence as input and was trained on five high-quality Hi-C datasets and Micro-C datasets to predict genome contact maps.|
    | **Key Results & Findings** <br>*(2-3 lines)* | 0.61 Pearson and ~0.56 Spearman correlation with real Hi-C data on unseen sequences, close to experimental replicate noise. CTCF motifs proved to be the single most important determinant of folding (removing them flattened predictions), motif orientation controlled loop position, and single-nucleotide changes near CTCF sites had measurable effects. It also correctly predicted real deletion experiments (Lmo2 locus), generalized partially to mouse DNA, and linked disease-associated SNPs to folding disruption.|
    | **Limitations Identified** <br>*(1-2 lines)* | Restricted to 1 Mb windows (no long-range or inter-chromosomal predictions), cannot predict A/B compartments, requires retraining per cell type, and has limited resolution for cell-type-specific differences.|
    | **Future Scope** <br>*(2-3 lines)* | Follow-up models building on Akita’s sequence-based 3D genome prediction include DeepC, C.Origami (which adds cell-type-specific signals such as CTCF binding), and AkitaV2, which improves interpretability by identifying influential CTCF sites. HiCPlus, published earlier, focuses on Hi-C resolution enhancement and is better viewed as parallel prior work rather than a follow-up. Akita has also enabled applications in evolutionary genomics and autism-related structural variant analysis.|
    | **Project Relevance** <br>*(1-2 lines)* | Demonstrates that sequence-only deep learning models can predict 3D genome structure and interpret disease variants through folding disruption rather than direct coding changes, useful as a baseline/comparison method for the current project.|
