# TorchResNet50MNIST

A PyTorch implementation of **ResNet-50** modified for the MNIST dataset (grayscale digit classification).

## Overview

This project trains a **ResNet-50** model on a subset of MNIST digits. The original ResNet-50 architecture was modified to:  
- Accept **grayscale images** (1 input channel)  
- Output **10 classes** (digits 0–9)  

Residual connections are retained for efficient training.

## Dataset

- MNIST subset:  
  - 1000 training samples  
  - 800 test samples  
- Images are transformed to tensors using `ToTensor()`  

## Training Details

- **Optimizer:** Adam (lr=0.003, weight decay=1e-5)  
- **Scheduler:** StepLR (decay factor 0.2 every 7 epochs)  
- **Loss Function:** Cross-Entropy Loss  
- **Epochs:** 30  
- **Batch size:** 32  

## Results

- Achieved **up to 96% accuracy** (may vary based on subset and random initialization)  

## Documentation

Detailed documentation is available as a PDF:  
[ResNet50_MNIST Documentation](docs/ResNet50_MNIST.pdf)
