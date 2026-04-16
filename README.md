
# VAMP-Net: Variant-Aware Multi-Path Network

**VAMP-Net** an Interpretable Multi-Path Fusion Architecture for *Mycobacterium tuberculosis* **MTB Drug Resistance Prediction**.

VAMP-Net addresses a critical gap in genomic modeling by disentangling biological causality from technical sequencing noise. By leveraging a Set Attention Transformer and a Quality-Aware CNN, the Nettwork provides robust, auditable resistance calls even for rare genomic variants.

## 🏗️ Architecture Overview
![VAMP-Net Architecture](https://github.com/Aicha-AI/VAMP-Net.MTB-Drug-Resistance/blob/main/Figures/model_architecture_detailed_new.png)
 
*Overview of the Multi-Path design.*

The **dual-pathway design**:

1. **Path 1 (Biological Topology):** Utilizes a **Set Attention Transformer (SAB)** to process genomic variant sequences as unordered sets. It captures high-order *epistatic interactions* while maintaining permutation invariance.
2. **Path 2 (Technical Confidence):** Employs a **Quality-Aware 1D-CNN** to process multi-channel VCF features (e.g., FRS, Depth), extracting patterns of sequencing reliability.

### 🔗 Adaptive Fusion
The outputs are integrated at a **Late Fusion Node** via an adaptive gating mechanism, allowing technical confidence to modulate biological findings for superior predictive performance.

## ✨ Key Features

* **Compositional Tokenization:** Handles rare/OOV variants by breaking them into fundamental sub-units (coordinates, nucleotides, delimiters).
* **Permutation Invariance:** Treats genomic mutations as a set rather than an artificial sequence.
* **Learnable Quality Aware:** Moves beyond binary VCF filters to learn from the continuous spectrum of sequencing confidence.
* **High Interpretability:** Attention maps and fusion gates provide clinical insights into "why" a resistance call was made.

## 📝 Citation
If you use this work in your research, please cite:

 Boutorh, Aicha, Kamar Hibatallah Baghdadi, and Anais Daoud. "VAMP-Net: An Interpretable Multi-Path Network of Genomic Permutation-Invariant Set Attention and Quality-Aware 1D-CNN for MTB Drug Resistance." arXiv preprint arXiv:2512.21786 (2026) 



## 🛠️ Installation
...

## 🏛️ Institutional Support
Developed at the National School of Artificial Intelligence (ENSIA)
Algiers, Algeria

