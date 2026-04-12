# Human Activity Recognition using Multimodal Fusion

This project investigates Human Activity Recognition (HAR) using accelerometer and gyroscope data from the UCI HAR dataset. It focuses on evaluating the impact of multimodal fusion strategies and comparing deep learning and traditional machine learning approaches.

---

## Overview

Human Activity Recognition is widely used in healthcare, smart environments, and wearable systems. This project explores whether combining multiple sensor modalities improves classification performance and robustness.

### Research Questions
- Does multimodal fusion improve performance over single-modality models?
- Which fusion strategy (early, mid, late) performs best?
- How do neural networks compare to traditional models on structured data?

---

## Methods

### Data
- Dataset: UCI Human Activity Recognition (UCI HAR)
- 10,299 samples with 561 engineered features
- Two modalities:
  - Accelerometer
  - Gyroscope

---

### Models Implemented
- Multi-Layer Perceptron (MLP)
- Support Vector Machine (SVM)
- XGBoost

---

### Fusion Strategies
- **Early Fusion**: Feature concatenation before training  
- **Mid Fusion**: Separate modality branches with feature-level fusion  
- **Late Fusion**: Ensemble of independent model predictions  

---

## Experimental Pipeline

1. Load dataset  
2. Separate accelerometer and gyroscope features  
3. Apply standardisation  
4. Train single-modality models  
5. Train multimodal fusion models  
6. Evaluate performance and compare results  

---

## Results Summary

- Multimodal fusion improves performance over single-modality models  
- SVM achieved the highest accuracy (~95%) on fused data  
- Mid and late fusion performed slightly better than early fusion  
- Differences between fusion strategies were not statistically significant  

---

## Key Findings

- Dataset characteristics strongly influence model performance  
- Traditional models outperform neural networks on structured features  
- Static activities (e.g., sitting vs standing) are hardest to classify  
- Fusion improves robustness but not dramatically on this dataset  

---

## Reproducibility

To reproduce the results:

### 1. Install dependencies
