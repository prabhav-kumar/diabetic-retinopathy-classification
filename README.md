# 🩺 Diabetic Retinopathy Binary Classification

This project classifies retinal images into two categories:

- **Yes** → DR Present (`Mild`, `Moderate`, `Severe`, `Proliferate_DR`)
- **No** → No DR (`No_DR`)

## 📦 Dataset

I used the [Diabetic Retinopathy 224x224 (2019) Dataset](https://www.kaggle.com/datasets/sovitrath/diabetic-retinopathy-224x224-2019-data) available on Kaggle.  
The original class distribution was as follows:

| Class            | Images |
|------------------|--------|
| No_DR            | 1805   |
| Mild             | 370    |
| Moderate         | 999    |
| Proliferate_DR   | 295    |
| Severe           | 193    |

To ensure class balance, I resampled the dataset to approximately 1400 images in total — 700 each for `Yes` and `No` categories. The dataset was split into **Train**, **Validation**, and **Test** sets.

---

## 📊 Results

### 🔒 Frozen ResNet50 Model

| Metric         | Train     | Validation | Test     |
|----------------|-----------|------------|----------|
| Accuracy       | 66.72%    | 86.50%     | 86.23%   |
| Loss           | 0.591     | 0.492      | 0.527    |

---

### 🔓 Fine-Tuned ResNet50 Model

| Metric         | Train     | Validation | Test     |
|----------------|-----------|------------|----------|
| Accuracy       | 91.88%    | 91.97%     | 93.12%   |
| Loss           | 0.227     | 0.214       | 0.171   |

---

## 📬 Model Access

To get the trained `.keras` model files (both frozen and fine-tuned), contact me at:  
📧 **k.prabhav2005@gmail.com**
