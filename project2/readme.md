# Ocular Disease Recognition using Deep Learning

**Final Grade:** **20 / 20**

---

## Project Overview
This project was developed for the course **Fundamentals of Machine Learning (FAA – 2025/26)** at the **University of Aveiro**.

The objective is **multi-label classification of ocular diseases** from **retinal fundus images**, addressing real-world challenges such as **class imbalance**, **co-occurring pathologies**, and **low-contrast medical images**.

The project evaluates the impact of **preprocessing strategies**, **model architecture**, and **decision calibration**, demonstrating that **data-centric design choices** are as critical as model complexity for clinically meaningful performance.

---

## Dataset
- **Source:** ODIR-5K (Ocular Disease Intelligent Recognition)
- **Total images:** ~5,000 fundus images
- **Diseases (8 classes):**
  - Normal
  - Diabetes
  - Glaucoma
  - Cataract
  - AMD
  - Hypertension
  - Myopia
  - Other
- **Task:** Multi-label classification (multiple diseases per image)
- **Key challenges:**
  - Severe class imbalance
  - Label co-occurrence
  - Low-contrast pathological features

---

## Models and Methods
- **EfficientNet-B0** (primary model – lightweight and efficient)
- **ResNet-50** (baseline comparison)
- **Ensemble architecture** (EfficientNet-B0 + MobileNetV3)
- **Transfer learning** with ImageNet pretrained weights
- **Loss functions:** Binary Cross-Entropy, Focal Loss
- **Explainable AI:** Grad-CAM for clinical interpretability

---

## Preprocessing Pipeline
Multiple preprocessing pipelines were evaluated:
- Image resizing and normalization
- Automated border cropping
- Data augmentation
- Adaptive contrast enhancement using **CLAHE**
- Patient-level data splitting to prevent leakage

CLAHE proved to be the most impactful preprocessing step, significantly improving detection of subtle vascular diseases.

---

## Results Highlights
- EfficientNet-B0 achieved **competitive macro F1-score** with **4–5× fewer parameters** than standard CNN baselines
- CLAHE increased model attention on vascular structures by **34%** (Grad-CAM analysis)
- Improved recall for minority diseases such as **Hypertension** and **Glaucoma**
- Demonstrated strong balance between **performance, efficiency, and interpretability**

---

## Kaggle Dataset Configuration

### 1. Generate Kaggle API Token
1. Go to your Kaggle profile: https://www.kaggle.com/
2. Open **Settings** → **API**
3. Click **Create New Token**
4. A `kaggle.json` file will be downloaded with the following format:

```json
{
  "username": "your_kaggle_username",
  "key": "your_kaggle_api_key"
}
