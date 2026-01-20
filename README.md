# Fundamentals of Machine Learning — Projects

This repository contains two projects developed for the course  
**Fundamentals of Machine Learning (FAA – 2025/26)** at the **University of Aveiro**.

Both projects focus on **medical image analysis**, combining solid theoretical foundations with practical Machine Learning and Deep Learning techniques, while using different computational environments according to project requirements.

---

## Project 1 — Brain Tumor Classification
**Grade:** **19.5 / 20**

### Description
Binary classification of brain tumors from **MRI images**, distinguishing between **tumor** and **no-tumor** cases.

### Development Environment
- Developed **locally** using **Anaconda**
- CPU-based training and evaluation
- No external GPU resources required

### Key Features
- Classical Machine Learning models (Logistic Regression, SVM, Neural Networks)
- Strong emphasis on preprocessing and feature separability
- Achieved **>99% accuracy** with SVM
- High interpretability and computational efficiency

### Techniques
- Image preprocessing (grayscale, histogram equalization, normalization)
- Linear vs. non-linear model comparison
- Statistical and visual performance analysis

---

## Project 2 — Ocular Disease Recognition
**Grade:** **20 / 20**

### Description
Multi-label classification of **ocular diseases** from retinal fundus images, addressing real-world clinical challenges such as **class imbalance** and **co-occurring pathologies**.

### Development Environment
- Developed using **Kaggle Notebooks**
- Use of **GPU acceleration** due to deep learning computational demands
- Kaggle API used exclusively for dataset access and training

### Key Features
- Deep Learning with EfficientNet-B0 and ResNet-50
- Advanced preprocessing (CLAHE, cropping, augmentation)
- Explainable AI using Grad-CAM
- Emphasis on efficiency, robustness, and clinical relevance

### Techniques
- Transfer learning
- Multi-label learning with sigmoid outputs
- Data-centric experimentation and statistical validation

---

## Technologies Used
- Python
- Anaconda (Project 1)
- NumPy, Scikit-learn
- PyTorch
- OpenCV
- Kaggle API (Project 2 — GPU support)
- Grad-CAM (Explainable AI)

---

## Authors
- **Carolina Silva** – MSc in Informatics Engineering (MEI) ([GitHub](https://github.com/carolinaspsilva2004))
- **Matilde Teixeira** – MSc in Computer and Telematics Engineering (MECT) ([GitHub](https://github.com/matildetex))  

**University of Aveiro**
