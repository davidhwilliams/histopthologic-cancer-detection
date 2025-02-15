# Histopathologic Cancer Detection

This repository contains code for the [Kaggle Histopathologic Cancer Detection Competition](https://www.kaggle.com/competitions/histopathologic-cancer-detection/overview), which focuses on identifying metastatic tissue in histopathologic scans of lymph node sections.

## Project Overview

The goal is to create an image classifier that can detect metastatic cancer in small image patches taken from larger digital pathology scans. The model predicts the probability that the center 32x32px region of a patch contains at least one pixel of tumor tissue.

## Dataset

The dataset consists of:

- **Training Set**: 220,000 images in .tif format with corresponding labels
- **Test Set**: 57,500 images for model evaluation
- **Labels**: Binary classification (0 = non-cancerous, 1 = cancerous)
- **Image Format**: TIF files containing histopathologic scans

## Model Evaluation

The model's performance is evaluated using the ROC AUC (Receiver Operating Characteristic Area Under the Curve) metric, which measures the trade-off between predicted probability and the observed target.

## Getting Started

1. Download the dataset from [Kaggle](https://www.kaggle.com/competitions/histopathologic-cancer-detection/data)
2. Install the required dependencies:

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import torch
```

3. Run the `kaggle-cancer.ipynb` notebook to train and evaluate the model
