# 📄 Paper 9: Geometric Deep Learning Framework for de Novo Genome Assembly
*   **Journal / Conference**: bioRxiv / Genome Research (2021/2025)
*   **DOI**: `10.1101/2024.03.11.584353`

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | The paper explores the idea of GNNome framework for path identification that corresponds to reconstructed genomic sequence, which is a critical stage of every de novo genome assembler. GNNome is based on geometric deep learning that enables training models on assembly graphs without relying on existing assembly strategies  |
| **Methodology & Approach** <br>*(2-3 lines)* | GNNome trains on graph neural networks (using SymGatedGCN layer), it reconstructs assemblies from PacBio, HiFi reads. The model learns to score each edge with a probability indicating how likely it is part of the correct genome assembly path. To build contigs, a search procedure starts from sampled edges and follows high-probability paths through the graph. Training uses a strand-symmetric loss and data augmentation techniques like masking and graph partitioning (e.g., METIS), with simulated reads generated from human reference chromosomes. |
| **Key Results & Findings** <br>*(2-3 lines)* | GNNome achieved contiguity (NG50/NGA50) comparable to or higher than the state-of-the-art assemblers like hifiasm, HiCanu, and Verkko across CHM13 genomes. The model generalized well to graphs 50× larger than those seen in training and could produce meaningful assemblies on ONT data despite being trained only on HiFi graphs. |
| **Limitations Identified** <br>*(1-2 lines)* | _The model showed higher misassembly counts on certain genomes compared to existing assemblers and produces lower QV (quality value) for CHM13. Also, direct transfer to a different type of data (ONT) is not the optimal solution and this approach is currently limited to haploid assembly. |
| **Future Scope** <br>*(2-3 lines)* | Future work aims to extend the framework to diploid and polyploid genome assembly, including aneuploid genomes relevant to cancer research, and to apply geometric deep learning to the overlap (graph construction) phase also, not just the path-finding phase. |
| **Project Relevance** <br>*(1-2 lines)* | The paper is methodologically relevant to our project’s Memory Efficient Assembly pillar as it validates our approach of applying graph-based deep learning for de novo path resolution rather than relying on existing algorithmic methods  |
