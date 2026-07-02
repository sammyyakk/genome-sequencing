# 📄 Paper 2: A universal SNP and small-indel variant caller using deep neural networks
*   **Journal / Conference**: Nature Biotechnology (2018)
*   **DOI**: `10.1038/nbt.4235`
*   **Link**: [Nature Biotechnology](https://www.nature.com/articles/nbt.4235)

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | The paper explores Deep Variant approach in which a deep CNN can call genetic variation in aligned next-gen sequencing ,read data by learning statistical relationship between images of read pileups around putative variant and true genotype calls. It has high sensitivity but low specificity. |
| **Methodology & Approach** <br>*(2-3 lines)* | DeepVariant encodes aligned reads and reference data around each candidate variant as an RGB pileup image, then applies a deep convolutional neural network (based on the Inception architecture) to classify each site into one of three diploid genotypes (hom-ref, het, hom-alt), replacing hand-crafted statistical models (used by tools like GATK) with a single learned model. |
| **Key Results & Findings** <br>*(2-3 lines)* | DeepVariant outperformed GATK, FreeBayes, SAMtools, 16GT, and Strelka on the NA24385 benchmark (SNP F1 = 99.95%, indel F1 = 98.98%), winning the FDA's Truth Challenge for SNPs, it has demonstrated more than 50% fewer errors per genome compared to the next-best method. The model is also generalized across genome builds (GRCh37, GRCh38), across species (human-trained model on mouse data outperformed mouse-trained model), and across sequencing technologies (Illumina, Ion Torrent, PacBio, SOLiD, 10X Genomics). |
| **Limitations Identified** <br>*(1-2 lines)* | Representing Variant calls as RGB images and applying deep CNN architecture to it is not possible in all cases as not all available read info can be encoded into three channel image.   |
| **Future Scope** <br>*(2-3 lines)* | Deep Variant’s key feature of generating entities with high sensitivity and low specificity and further applying deep learning to assign biological labels to it can be applicable to other high-throughput instruments. High accuracy can be achieved through better pre-processing steps than the model itself. |
| **Project Relevance** <br>*(1-2 lines)* | It is relevant to our Whole Genome Sequencing pillar - DeepVariant is the foundational deep convolutional network approach for variant calling which our project builds on. |
