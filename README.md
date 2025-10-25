# Prodigy ML Internship – Task 3  
**Cat vs. Dog Image Classification using SVM**

---

### Objective
Implement a **Support Vector Machine (SVM)** classifier to distinguish between cat and dog images from the Microsoft Cats vs Dogs dataset.  
- Preprocess images (resize, flatten, PCA for dimensionality reduction).  
- Train on a subset for efficiency.  
- Evaluate accuracy and classification metrics.  

This task demonstrates computer vision basics with classical ML (no deep learning).

---

### Dataset
- **Source**: [Kaggle – Microsoft Cats vs Dogs](https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset)  
- **Size**: ~25,000 images (12,500 cats + 12,500 dogs)  
- **Format**: JPEG files in `PetImages/Cat` and `PetImages/Dog` folders  
- **Download via Kaggle API** in the notebook  

Note: Dataset inspired by the original ASIRRA challenge for CAPTCHA-like tasks.

---

### Key Results
| Metric          | Value (on Test Set) | Interpretation |
|-----------------|---------------------|----------------|
| Accuracy       | ~55%               | Moderate; limited by classical SVM on raw pixels – CNNs would improve to 90%+ |
| Precision (Cat)| 0.57               | Balanced classes |
| Recall (Cat)   | 0.51               | Some misclassifications |
| F1-Score (Cat) | 0.54               | Room for optimization (e.g., better features) |
| Precision (Dog)| 0.54               | Similar performance |
| Recall (Dog)   | 0.59               | |
| F1-Score (Dog) | 0.56               | |

Results from linear SVM on PCA-reduced features (100 components) using a 500-image subset for training.

---

### Repository Files
