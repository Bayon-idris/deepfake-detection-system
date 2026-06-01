# Deepfake Detection System

## Description
This repository reproduces the LAA-Net (CVPR 2024) baseline for deepfake detection 
as a starting point for my research project.

Original paper: [LAA-Net: Localized Artifact Attention Network for Quality-Agnostic 
and Generalizable Deepfake Detection](https://arxiv.org/pdf/2401.13856.pdf)

Original repository: https://github.com/10lcool10BRAVO/LAA-Net

## Setup & Reproduction Notes
Several compatibility fixes were needed to run on our environment 
(CUDA 12.0, RTX 3060, NumPy >= 1.24):
- Fixed `np.bool` deprecation
- Fixed bbox float-to-int casting
- Fixed `initial_lr` in scheduler
- Adapted dataset paths for FF++ c23

## Training (SBI)
```bash
./scripts/efn_sbi.sh
```

## Testing
```bash
./scripts/test_sbi.sh
```

## Based on
Nguyen et al., LAA-Net, CVPR 2024