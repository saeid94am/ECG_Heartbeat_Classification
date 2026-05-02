# ECG Arrhythmia Classification using GA-Optimized 1D CNN

This repository presents an end-to-end deep learning framework for ECG-based heartbeat classification, based on an enhanced version of my Master's thesis and associated research work.

## Overview

This project proposes a lightweight 1D Convolutional Neural Network (CNN) optimized via a Genetic Algorithm (GA) for accurate and efficient arrhythmia classification. The model follows an end-to-end pipeline with minimal preprocessing and no handcrafted feature extraction.

## Key Contributions

* GA-based hyperparameter optimization for CNN architecture
* Class-aware data augmentation strategy for imbalanced ECG data
* Lightweight architecture with competitive performance
* End-to-end learning directly from raw heartbeat signals

## Dataset

The model is trained and evaluated on the MIT-BIH Arrhythmia dataset.

Dataset source:
Kachuee et al., *"ECG Heartbeat Classification: A Deep Transferable Representation"*

Kaggle link:
https://www.kaggle.com/datasets/shayanfazeli/heartbeat

## Methodology

* Signal preprocessing and heartbeat extraction (187 samples per beat)
* Class-aware augmentation (noise injection + amplitude modulation)
* Genetic Algorithm for optimizing:

  * Number of filters
  * Kernel size
  * Stride
  * Dropout rate
  * Learning rate

## Results


The model demonstrates strong performance, particularly on minority classes, while maintaining low computational complexity.

## Repository Structure

* `notebook` — Includes Main implementation
* `README.md` — Project documentation
* `requirements.txt` - dependencies
* `mitbih` — Data directory
* `img` - result images directory


## Requirements

python==3.10.11

Install dependencies using:

pip install -r requirements.txt
