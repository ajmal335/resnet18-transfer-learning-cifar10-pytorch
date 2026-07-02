# Transfer Learning with ResNet18 on CIFAR-10 (PyTorch)

## Project Overview

This project demonstrates transfer learning using a pretrained ResNet18 model in PyTorch for image classification on the CIFAR-10 dataset.

Instead of training the entire network from scratch, all pretrained layers are frozen, and only the final fully connected classification layer is trained.

This approach significantly reduces training time while improving accuracy compared to a custom CNN.

---

## Dataset

CIFAR-10 contains 60,000 RGB images (32×32) across 10 classes:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

---

## Transfer Learning Workflow

Input Image

↓

Resize (224×224)

↓

Data Augmentation

↓

ImageNet Normalization

↓

Pretrained ResNet18

↓

Freeze All Layers

↓

Replace Final Fully Connected Layer

↓

Train Only Classifier

↓

Prediction

---

## Features

- Pretrained ResNet18
- Feature Extraction
- Image Resizing
- Data Augmentation
- ImageNet Normalization
- CrossEntropy Loss
- Adam Optimizer
- GPU Support
- Model Saving

---

## Technologies

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib

---

## Results

Test Accuracy: **81%**

---

## Future Work

- Fine-Tuning ResNet18
- Learning Rate Scheduler
- Early Stopping
- Mixed Precision Training
- Gradual Unfreezing
