# 🌱 Soil Image Classification Challenge

This repository contains solutions to the soil classification task, including both **binary classification** (soil vs. non-soil) and **multi-class classification** (different soil types). We use deep learning models like **ResNet18** and **EfficientNet-B0** along with preprocessing and ensembling techniques to boost performance.

---

## 📁 Repository Structure

├── notebooks/
│ ├── soil-classification-part1.ipynb
│ └── soil classification 2.ipynb
├── docs/
│ ├── Soil Image Classification Part 1.pdf
│ └── soil classification 2 report.docx
├── README.md
├── requirements.txt


---

## 🔍 Tasks Covered

### 1. **Binary Classification** (EfficientNet)
- Merges two datasets (soil and digit images)
- Applies robust preprocessing (smart cropping, CLAHE, augmentation)
- Uses EfficientNet-B0 with class-balanced loss
- Ensemble of 3 models via boosting
- Output: Predicts whether an image is *soil* or *not-soil*

### 2. **Multi-class Classification** (ResNet18)
- Works with 4 soil types from labeled dataset
- Uses label encoding and class weights
- Strong augmentations for better generalization
- Uses ResNet18 with boosting (min-F1 optimization)
- Output: Predicts the correct soil type (Alluvial, Black, Clay, Red)

---

## 🧠 Models Used

| Model           | Task                      | Ensemble | Optimized For       |
|-----------------|---------------------------|----------|---------------------|
| EfficientNet-B0 | Binary Classification     | ✅ Yes   | F1 Score            |
| ResNet-18       | Multi-class Classification| ✅ Yes   | Minimum Class-wise F1 |

---

## 🔧 How to Use

1. Clone the repository:

```bash
git clone https://github.com/yourusername/soil-classification-challenge.git
cd soil-classification-challenge
