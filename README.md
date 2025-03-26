# Fine-Tune Image Classification with PyTorch

## Overview
This example demonstrates how to fine-tune a pre-trained ResNet18 model on the CIFAR10 dataset using PyTorch. The project includes loading a pre-trained model, modifying its architecture, freezing layers, training on a custom dataset, and evaluating performance.

---

## Features
- **Pre-trained Model**: Uses `ResNet18` from `torchvision` (pre-trained on ImageNet).
- **Dataset**: CIFAR10 (10-class image classification).
- **Fine-Tuning Workflow**:
  - Modify the final fully connected layer for 10 classes.
  - Freeze early layers to retain pre-trained features.
  - Train only the modified layers (optionally unfreeze later).
- **Training Metrics**: Logs loss and accuracy.

---

## Requirements
- Python 3.8+
- PyTorch 2.0+
- torchvision 0.15+
- CUDA 11.8 (recommended for GPU training)
- Libraries:
  ```bash
  pip install torch torchvision tqdm

# Troubleshooting
Issue	Solution
CUDA Out of Memory	Reduce batch_size (e.g., 16 instead of 32)
Dataset Download Failed	Check internet connection or manually download CIFAR10
Slow Training	Enable GPU (device = "cuda")
# License
MIT License. See LICENSE for details.
