**Project Overview**
This repository implements an automated Forest Fire Detection pipeline using computer vision and deep learning. The goal is to detect fire and smoke from images (or short videos/frames) captured by surveillance cameras, drones, or satellites and raise alerts for early intervention.
The project contains data preprocessing, model training (from-scratch CNN and transfer learning options), evaluation scripts, and inference utilities for deploying the model in a real-time system.
**Key Features**

Binary classification: fire/smoke vs no-fire (configurable for multi-class)
Data augmentation for robustness (rotation, flip, brightness changes, etc.)
Support for transfer learning (MobileNetV2, ResNet, EfficientNet) and custom CNNs
Training, validation, and test pipelines with logging and model checkpointing
Inference script for single images and video streams
Metrics: accuracy, precision, recall, F1-score, ROC AUC

**Dataset**

Note: Replace this with your dataset details (source, license, size).
Typical datasets used:
Custom collected images from drones/cameras
Public datasets (e.g., “Forest Fire Image Dataset”, dataset links)

Dataset structure expected:
dataset/
  train/
    fire/
    no_fire/
  val/
    fire/
    no_fire/
  test/
    fire/
    no_fire/
    
**Methodology**

Collect & label images into fire and no_fire classes.

Preprocess: resize, normalize, augment.

Train model using transfer learning or a custom CNN.

Validate and tune hyperparameters.

Evaluate on held-out test set and perform error analysis.

Deploy inference pipeline for images / video frames.

**Preprocessing**

Resize images to a consistent size (e.g., 224×224)

Normalize to ImageNet or custom mean/std
