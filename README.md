# 🖼️ Real vs AI-Generated Image Textures: A Machine Learning Study

This repository contains our project on **distinguishing real images from AI-generated images** using **texture-based features** and a variety of **machine learning models**.  
The work compares multiple classifiers and explores dimensionality reduction techniques to optimize performance.

---

## 📌 Problem Statement
With the rise of **GANs** and **diffusion models**, AI-generated images have become increasingly realistic. While this has advanced digital creativity, it also introduces risks such as:
- Misinformation  
- Identity theft  
- Misuse in cybersecurity  

This project investigates whether **texture-based features** (GLCM, LBP, wavelet transforms, PCA) can be effectively used to **distinguish real vs AI-generated images**.

---

## 📂 Repository Contents
- **Dataset** → Real vs AI-Generated Image Texture Feature Dataset (Kaggle).  
- **Code** → Preprocessing, feature selection, PCA, and ML models.  
- **Presentation (PDF)** → Project presentation slides.  
- **README.md** → Project overview (this file).  

---

## 🧾 Dataset
- **Source**: [Kaggle Dataset: Real vs AI-Generated Image Texture Feature Dataset](https://www.kaggle.com/datasets/arkanivasarkar/real-vs-ai-generated-image-texture-feature-dataset)  
- **Size**: 66,898 rows × 123 columns  
- **Distribution**:  
  - 33,477 Real images  
  - 33,421 AI-generated images  
- **Features**: 122 float features + 1 label column  

---

## ⚙️ Methodology
1. **Data Preprocessing**
   - Removal of unnecessary features  
   - Handling missing values  
   - Outlier detection and capping (IQR method)  
   - Standardization of features  

2. **Dimensionality Reduction**
   - **Feature Selection**: Pearson Correlation (top 12 features, 91.03% variance explained)  
   - **PCA**: 4 Principal Components (95.35% variance explained)  

3. **Models Implemented**
   - Logistic Regression  
   - Random Forest Classifier  
   - Naïve Bayes  
   - K-Nearest Neighbours (KNN)  
   - Support Vector Machines (SVM: Linear, Polynomial, RBF)  

4. **Evaluation Metrics**
   - Confusion Matrix  
   - Accuracy  
   - Precision & Recall  
   - F1-score  

---

## 📊 Results & Key Insights
- **Feature Selection**:  
  - Random Forest performed best → **81% accuracy**.  

- **Feature Extraction (PCA)**:  
  - SVM (RBF kernel) performed best → **80.75% accuracy**.  

- Logistic Regression, Naïve Bayes, and KNN showed **moderate performance** compared to Random Forest and SVM.  

---

## 🎯 Conclusion
- Texture-based features are a **viable method** to distinguish AI-generated images.  
- Both **Feature Selection** and **PCA** effectively reduced dimensionality while preserving accuracy.  
- **SVM (RBF kernel)** and **Random Forest** emerged as the top classifiers for this task.  

---

## 🖼️ Project Presentation
📑 [View Presentation Slides](TeamA_CAC2_PPT (1).pdf)

---

## 👥 Team
**Team A**  
- Project Contributors: Shrutika Gupta, Puspita Biswas, Agrawal Raj, Jaya Mary Jennifer D., Harsha K. 
- Department of Computer Science, CHRIST(Deemed to be University), Bangalore, Yeshwanthpur Campus  

---
