# 📄 Paper 7: DeepSignal: Detecting DNA Methylation State from Nanopore Sequencing Reads Using Deep-Learning
*   **Journal / Conference**: Bioinformatics (2019)
*   **DOI**: `10.1093/bioinformatics/btz276`

---

## 🔬 Literature Review Table

| Evaluation Field | Researcher Analysis |
| :--- | :--- |
| **Problem Addressed** <br>*(1-2 lines)* | Earlier tools that read these signals used HMM (hidden Markov models), which is an older statistical method, not deep learning. These were less accurate and needed a lot of read coverage to work properly so Detecting DNA methylation (5mC and 6mA) directly from Nanopore sequencing signals was still inaccurate and inefficien.|
| **Methodology & Approach** <br>*(2-3 lines)* |  Built deep signal , a deep learning model made uo of a two feature extraction modules combined into one classifer. A CNN reads the raw electrical signal values around a target base to capture its shape while a BRNN reads the surrounding dna sequence plus both signal statistics to capture sequence context, both are combined and sent to a fully connected neural network that finds whether the base is methylated or not.|
| **Key Results & Findings** <br>*(2-3 lines)* | : DeepSignal beat HMM-based tools (nanopolish, signalAlign) on accuracy, sensitivity, specificity, and AUC across all tested organisms, needing far less coverage (90%+ accuracy at just 2x vs. 30x+ for older methods). It reached above 0.9 Pearson correlation with bisulfite sequencing at just 20x coverage, and even detected ~5% more CpG sites than bisulfite sequencing, especially in centromeric regions. |
| **Limitations Identified** <br>*(1-2 lines)* |DeepSignal needs to be retrained for each new type of base modification, since it currently only handles 5mC and 6mA. It also still struggles in some repetitive/centromeric regions, where a portion of CpGs remained undetectable even for DeepSignal. |
| **Future Scope** <br>*(2-3 lines)* | The authors plan to train DeepSignal on more types of base modifications as more training data becomes available, since it currently only detects 5mC and 6mA. They also suggest it could be used to further study the functional role of methylation in centromeric regions, and more broadly to improve understanding of epigenetic mechanisms in processes like aging, cancer, and neural development. |
| **Project Relevance** <br>*(1-2 lines)* |Demonstrates how deep learning (CNN + RNN combined) can be applied to raw biological signal data, not just DNA sequence alone, to predict epigenetic states relevant as a comparison point for how different architectures (CNN-only in Akita vs. CNN+BRNN here) handle sequence-to-function prediction tasks in genomics. |
