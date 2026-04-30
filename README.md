# CNN Image Classifier — CIFAR-10

**Student:** Aman Gill | UB: 23055704
**Module:** COS6031-D Applied AI Professional — Portfolio Evidence
**Level:** Semi-Complex Project
**Date:** April 2026

---

## What this does

A Convolutional Neural Network built from scratch in PyTorch
to classify images into 10 categories using CIFAR-10.

## How to run

Open the notebook in Google Colab and run all cells in order.

## Results

- Overall Test Accuracy: 79.36%
- Correct predictions: 7936 / 10000
- Best class: Automobile 93.4%
- Hardest class: Dog 62.0%
- Training epochs: 10
- Final training accuracy: 82.69%

## Architecture

- Conv Layer 1: 32 filters, 3x3, BatchNorm, ReLU, MaxPool
- Conv Layer 2: 64 filters, 3x3, BatchNorm, ReLU, MaxPool
- Conv Layer 3: 128 filters, 3x3, BatchNorm, ReLU, MaxPool
- FC1: 2048 to 512, ReLU, Dropout 0.5
- Output: 512 to 10 classes

## What I used

- Python, PyTorch, torchvision, NumPy, Matplotlib
- CIFAR-10 dataset (60,000 colour images, 10 classes)

## What I learnt

Building this from scratch made the CNN architecture tangible
in a way that using pre-trained YOLO in AVC&C did not. Every
architectural decision had a visible effect on accuracy.
Dropout was the single most impactful change — without it
training accuracy hit 90% but test was only 65%.
This directly informed how I think about the YOLO11n model
in AVC&C — both use the same convolutional building blocks.

## Files

- `CNN_Image_Classifier.ipynb` — full notebook with outputs
