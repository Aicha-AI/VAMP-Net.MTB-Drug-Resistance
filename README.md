
# VAMP-Net: Variant-Aware Multi-Path Network

**VAMP-Net** is a deep learning framework designed to predict drug resistance in *Mycobacterium tuberculosis* by disentangling biological signals from technical noise.

## 🏗️ Architecture Overview
![VAMP-Net Architecture](https://github.com/Aicha-AI/VAMP-Net.MTB-Drug-Resistance/blob/main/Figures/model_architecture_detailed_new.png)
 
*Overview of the Multi-Path design.*

The framework employs a **dual-pathway design**:

1. **Path 1 (Biological Topology):** Utilizes a **Set Attention Transformer (SAB)** to process genomic variant sequences as unordered sets. It captures high-order *epistatic interactions* while maintaining permutation invariance.
2. **Path 2 (Technical Confidence):** Employs a **Quality-Aware 1D-CNN** to process multi-channel VCF features (e.g., FRS, Depth), extracting patterns of sequencing reliability.

### 🔗 Adaptive Fusion
The outputs are integrated at a **Late Fusion Node** via an adaptive gating mechanism, allowing technical confidence to modulate biological findings for superior predictive performance.

## 🛠️ Installation
```bash
git clone [https://github.com/YourUsername/VAMP-Net.git](https://github.com/YourUsername/VAMP-Net.git)
cd VAMP-Net
pip install -r requirements.txt
