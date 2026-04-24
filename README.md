# Underwater Image Classification using Deep Learning

This repository presents a comparative study between different deep learning approaches for underwater image classification using the AQUA20 dataset.

## 📌 Models Evaluated

- ResNet-18 (CNN baseline)
- YOLOv8 (classification mode)
- MVELSA (proposed method)

## 🧠 Key Idea

We investigate how different feature extraction strategies behave under challenging underwater conditions, particularly in scenarios with:

- High visual variability (noise, turbidity, illumination changes)
- Strong class imbalance
- Limited labeled data

The proposed MVELSA approach leverages multiple latent representations to improve classification performance under these constraints.

---

## 📦 Dataset

We use the **AQUA20 dataset**, which contains 20 classes of underwater organisms and exhibits strong class imbalance.

### 📥 Download Instructions

You can download the dataset directly using the Hugging Face `datasets` library:

```python
# Install dependencies
!pip install datasets
!pip install torch torchvision

# Load dataset
from datasets import load_dataset

dataset = load_dataset("taufiktrf/AQUA20")
