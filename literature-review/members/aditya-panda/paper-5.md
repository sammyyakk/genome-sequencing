# 📄 Paper 5: Predicting Splicing from Primary Sequence with Deep Learning
*   **Journal / Conference**: Cell (2019)
*   **DOI**: `10.1016/j.cell.2018.12.015`
*   **Link**: [Cell](https://www.cell.com/cell/fulltext/S0092-8674(18)31629-5)

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** | Older splice-prediction tools relied on short local sequence windows, so they could flag canonical splice sites but missed the broader genomic context that governs splicing. As a result they overlooked many disease-causing splicing mutations, especially cryptic and deep-intronic variants that sit far from obvious splice junctions. |
| **Methodology & Approach** | SpliceAI is a 32-layer residual neural network that takes raw DNA sequence as input, with no hand-engineered biological features, and predicts for each nucleotide the probability that it is a splice donor, acceptor, or neither. It evaluates roughly 10 kb of surrounding context, which is what lets it capture the long-range regulatory signals that older, small-window models cannot see. |
| **Key Results & Findings** | SpliceAI substantially outperformed previous tools, identifying both canonical splice sites and the harder cryptic and non-canonical events. Its wide sequence context let it detect variants far from exon and intron boundaries, including deep-intronic mutations that older approaches missed. Predicted splice-altering de novo mutations validated against patient RNA-seq in 21 of 28 (about 75%) autism and intellectual-disability cases, and the authors estimated that 9 to 11% of pathogenic mutations in rare genetic disorders arise from this previously underappreciated class of splicing disruption. |
| **Limitations Identified** | SpliceAI produces a single consensus prediction and does not model tissue-specific splicing, even though the same gene can be spliced differently across cell types. Its sensitivity also falls for deep-intronic variants, and because it is trained on existing gene annotations, it inherits whatever gaps or biases those annotations contain. |
| **Future Scope** | A natural next step is tissue-specific splicing models that account for regulatory differences across cell types, directly addressing SpliceAI's main blind spot. Combining splice predictions with gene-expression, protein-function, and clinical evidence would enable more complete variant interpretation, strengthening the role of AI-based splicing prediction in routine clinical genomics and rare-disease diagnosis. |
| **Project Relevance** | SpliceAI recovers an entire category of pathogenic variants, the splice-disrupting ones, including cryptic and deep-intronic mutations that conventional calling and filtering pipelines routinely miss. Its delta scores can plug into our pipeline as an additional prioritization signal, helping surface likely-pathogenic variants from large-scale whole-genome sequencing data and directly supporting Problem 3. |
