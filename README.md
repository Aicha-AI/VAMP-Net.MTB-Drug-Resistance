# VAMP-Net 🧬
## Variant-Aware Multi-Path Network for Drug Resistance Prediction

The framework employs a dual-pathway design to disentangle biological signal from technical noise. Path
1 (Biological Topology) utilizes a Set Attention Transformer (SAB) to process genomic vari-
ant sequences as unordered sets; the multi-head attention mechanism captures high-order epistatic
interactions between mutations while maintaining permutation invariance. Simultaneously, Path 2
(Technical Confidence) employs a Quality-Aware 1D-CNN to process multi-channel VCF features,
extracting local patterns of sequencing reliability. The outputs of both paths are integrated at a Late
Fusion Node via an adaptive gating mechanism, allowing technical confidence to modulate biolog-
ical findings. The fused representation is finally processed by a Classification Head consisting of
fully connected layers and dropout regularization to produce the final drug resistance prediction.
