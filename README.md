# Early-Onset Alzheimer’s Detection Using Multi-Modal Data Fusion of Retinal Imaging, Speech Patterns, and Genomic Data

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Framework: PyTorch](https://img.shields.io/badge/Framework-PyTorch-orange.svg)](https://pytorch.org/)
[![Domain: Multimodal Healthcare](https://img.shields.io/badge/Domain-Multimodal%20Healthcare--NeuroAI-red.svg)]()

This repository hosts the official research and implementation of a cutting-edge **Multi-Modal Data Fusion Framework** engineered for the ultra-early detection of Early-Onset Alzheimer's Disease. By cross-analyzing and fusing three non-invasive, distinct biological markers—**Retinal Images (Computer Vision)**, **Speech Patterns (Audio/NLP)**, and **Genomic Data (Bioinformatics)**—this framework is designed to identify subtle neurodegenerative patterns up to 5 years before conventional cognitive symptoms manifest.

---

## 📌 Research Vision & Core Concept
Single-modality diagnostic tools (like relying only on MRI scans) often catch Alzheimer's when significant, irreversible brain damage has already occurred. This project introduces a holistic, multi-perspective approach:
* **Retinal Imaging:** Tracking microvascular changes and nerve fiber layer thinning in the eye (acting as a direct window to the brain).
* **Speech Patterns:** Evaluating acoustic degradation, pauses, and linguistic choices using speech-to-text and acoustic feature extractors.
* **Genomic Data:** Analyzing Single Nucleotide Polymorphisms (SNPs) and high-risk genetic variations (such as the APOE ε4 allele).
* **Cross-Modal Data Fusion:** Merging these heterogeneous feature spaces using advanced Cross-Attention mechanisms or Early/Late Fusion layers.

---

## 🛠️ Key Features & Methodology
1. **Multi-Modal Feature Extractors:** Custom neural pipelines featuring CNNs/Vision Transformers (for Retinal Images), Wav2Vec/BERT (for Speech), and Feed-Forward Embedding nets (for Genomics).
2. **Advanced Fusion Network:** Implements a Transformer-based cross-attention mechanism that learns correlation weights across different data modalities.
3. **Imbalanced Class Optimization:** Custom loss functions (Focal Loss/Contrastive Loss) optimized for early-stage diagnostic data scarcity.
4. **Gold Standard Benchmarking:** Ready-made integration pipelines for world-renowned medical repositories including the **ADNI (Alzheimer's Disease Neuroimaging Initiative)** and **UK Biobank**.

---

## 📂 Repository Structure
```text
├── src/
│   ├── data_processors/    # Separate data loaders for Images, Audio, and Genomic text
│   ├── encoders/           # Specific feature extractors (Vision, NLP, Bio)
│   ├── fusion_layers/      # Cross-attention and multi-modal merging pipelines
│   └── evaluation/         # ROC-AUC curves, Confusion Matrices, and F1 scoring
├── data/                   # Preprocessing configurations for ADNI data splits
├── configs/                # Hyperparameters for training epochs and fusion types
├── notebooks/              # Exploratory data fusion and feature visualization
├── Literature_Review/      # Team research matrices and BibTeX references
└── README.md
