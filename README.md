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
- <img width="641" height="556" alt="image" src="https://github.com/user-attachments/assets/dbe4789e-be14-4690-b076-e4244f92893d" />
- <img width="846" height="683" alt="image" src="https://github.com/user-attachments/assets/2ee313d9-847e-46ea-aca8-5b6e1e985731" />
- <img width="846" height="683" alt="image" src="https://github.com/user-attachments/assets/e60be7c9-09fc-42db-8136-c22d87be5363" />
- <img width="854" height="683" alt="image" src="https://github.com/user-attachments/assets/4eb3bd2b-6a46-4725-bc19-bbb45d26615d" />





## Documentation & Notebook

- Detailed documentation is available as a PDF:  
[ResNet50_MNIST Documentation](ResNet-50%20for%20MNIST%20Model%20Overview%20and%20Training%20Summary.pdf)
- Jupyter Notebook: 
[View Notebook on GitHub](TorchResNet50MNIST.ipynb)  
- Run the notebook on Google Colab: 
[Open in Colab](https://colab.research.google.com/github/powervnc/TorchResNet50MNIST/blob/main/TorchResNet50MNIST.ipynb)


