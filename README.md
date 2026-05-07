# CluDis: Unsupervised Disentangled Representation Learning via Clustering-based Guidance and Latent Diffusion

This repository contains the official implementation of **CluDis**, an unsupervised disentangled representation learning framework that combines clustering-based pseudo-factor discovery, cluster-to-latent injection, and conditional latent diffusion autoencoding.

> **Note:** The codebase is currently being organized and cleaned for public release.  
> Core implementation files, training scripts, pseudo-label construction scripts, and evaluation protocols will be progressively updated in this repository.

## Framework Overview

CluDis aims to construct a semantically controllable latent space without relying on manual attribute annotations. The overall framework consists of three main components:

1. **Clustering-based Pseudo-factor Discovery (CPD)**  
   Extracts patch-level visual representations from a frozen pretrained visual encoder and performs dataset-level clustering to obtain cluster-guided pseudo-labels.

2. **Cluster-to-Latent Injection (CLI)**  
   Injects the discovered pseudo-labels into a designated attribute latent subspace, establishing a deterministic correspondence between pseudo-factors and traversal dimensions.

3. **Conditional Latent Diffusion Autoencoding (CLDA)**  
   Uses a conditional latent diffusion reconstruction backbone to preserve high-fidelity visual details while maintaining the structured latent representation.

<p align="center">
  <img src="Framework.png" width="95%">
</p>

## Repository Status

This repository is under active organization. The following components will be released step by step:

- [ ] Environment setup instructions
- [ ] Dataset preparation scripts
- [ ] DINOv2 feature extraction scripts
- [ ] Clustering-based pseudo-label construction
- [ ] CluDis training code
- [ ] Reconstruction and traversal scripts
- [ ] Evaluation code for FID, PSNR, PPL, MIG, DCI, and Modularity
- [ ] Pretrained checkpoints and example outputs

## Expected Directory Structure

```text
CluDis/
├── README.md
├── figures/
│   └── framework.png
├── configs/
├── datasets/
├── models/
├── scripts/
├── train.py
├── eval/
└── requirements.txt
