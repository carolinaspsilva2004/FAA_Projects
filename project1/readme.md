# Brain Tumor Classification using Machine Learning

**Final Grade:** **19.5 / 20**

---

## Project Overview
This project was developed for the course **Fundamentals of Machine Learning (FAA – 2025/26)** at the **University of Aveiro**.  
The goal is the **binary classification of brain tumors** from **Magnetic Resonance Imaging (MRI)** scans, distinguishing between **tumor** and **no-tumor** cases.

The work demonstrates that **classical Machine Learning algorithms**, when combined with a **carefully designed preprocessing pipeline**, can achieve **near state-of-the-art performance**, rivaling deep learning approaches while remaining interpretable and computationally efficient.

---

## Objectives
- Develop a reliable binary classifier for brain tumor detection from MRI images  
- Compare linear and non-linear Machine Learning models  
- Evaluate performance using accuracy, precision, recall, and F1-score  
- Study the impact of preprocessing and model complexity on classification results  

---

## Dataset
- **Source:** Brain Tumor MRI Dataset (Kaggle)  
- **Total images:** 6,726  
- **Original classes:** glioma, meningioma, pituitary, no tumor  
- **Final classes:** tumor vs. no tumor  
- **Image resolution:** 128 × 128  
- **Data split:**
  - Training: 5,521 images  
  - Testing: 1,205 images  
- **Class balance:** Moderately imbalanced (~74% tumor)

---

## Preprocessing Pipeline
The following preprocessing steps were applied to improve data quality and class separability:
- Duplicate image removal (297 images)
- Conversion to grayscale
- Resizing to 128×128 pixels
- Histogram equalization for contrast enhancement
- Min–max normalization to the range [0, 1]
- Statistical analysis of intensity distributions

This pipeline was a key factor in achieving the high classification performance.

---

## Models Evaluated

### Logistic Regression
- Linear classifier with L2 regularization  
- Test accuracy: **99.34%**  
- High interpretability through learned weight maps  

### Neural Network
- Fully connected architecture with one hidden layer (64 neurons)  
- Implemented from scratch using NumPy  
- Test accuracy: **98.01%**  
- Strong recall, but affected by overfitting during cross-validation  

### Support Vector Machine (SVM)
- Polynomial kernel (degree 2)  
- Test accuracy: **99.59%**  
- Best overall performance and generalization ability  

---

## Results Summary
| Model | Accuracy |
|------|----------|
| Logistic Regression | 99.34% |
| Neural Network | 98.01% |
| **SVM (Polynomial)** | **99.59%** |

- All models achieved accuracy above **98%**
- The polynomial SVM provided the best trade-off between precision, recall, and stability
- Logistic Regression proved that simple linear models can be extremely effective when paired with strong preprocessing

---

## Conclusions
- Data quality and preprocessing are critical in medical image classification tasks  
- Classical Machine Learning models can match or surpass more complex deep learning approaches in binary MRI tumor classification  
- The SVM achieved the strongest overall results  
- Logistic Regression offers an excellent interpretable and computationally efficient alternative  
- The Neural Network requires improved regularization to enhance robustness  

---

## Future Work
- Extend the framework to multi-class tumor classification  
- Explore CNN-based models and transfer learning  
- Integrate Explainable AI techniques (e.g., Grad-CAM, LIME)  
- Validate the models on multi-institutional clinical datasets  

---

## Authors
- **Carolina Silva** – MSc in Informatics Engineering (MEI) ([GitHub](https://github.com/carolinaspsilva2004))
- **Matilde Teixeira** – MSc in Computer and Telematics Engineering (MECT) ([GitHub](https://github.com/matildetex))  
**University of Aveiro**

**University of Aveiro**
