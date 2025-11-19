# 🧠 Brain Tumor Classification from MRI Scans

This project applies **machine learning and computer vision techniques** to classify brain tumors from MRI scans. The goal is to assist clinicians in improving the speed and accuracy of diagnosis through automated multi-class classification.

---

## 🎯 Objectives
- Perform **automated feature extraction** from MRI scans.  
- Train and evaluate models to classify tumors into **Meningioma, Glioma, Pituitary Tumor, or No Tumor**.  
- Compare models for performance and interpretability to select the most effective diagnostic approach.  

---

## 🛠️ Methodology & Modeling Approach
### 1. Data Preprocessing & Augmentation
- **Image Handling:** Load, resize, and normalize MRI scans using OpenCV (`cv2`) and PIL.  
- **Feature Extraction:** Convert high-dimensional images into vectors using classical techniques or CNN embeddings.  

### 2. Supervised Classification
- **K-Nearest Neighbors (KNN):** Baseline non-parametric model.  
- **Random Forest (RF):** Ensemble tree-based model for robustness.  
- **Support Vector Machine (SVM):** Finds optimal hyperplanes for tumor class separation.  
- **CNN & CNN+Attention:** End-to-end deep learning models for high-accuracy classification.  
- **ResNet-50:** Advanced deep learning model leveraging residual connections.  

### 3. Model Evaluation
- Accuracy, F1-Score, Confusion Matrix for multi-class assessment.  
- CNN+Attention achieved **90% overall accuracy** and **weighted F1-score 0.90**.  
- SVM baseline achieved **74% accuracy**.

---

## 💻 Technologies & Libraries
| Category | Library | Purpose |
|----------|---------|--------|
| Data Analysis | pandas, numpy | Load and manipulate MRI image metadata |
| Image Processing | cv2 (OpenCV), PIL | Read, resize, normalize MRI images |
| Machine Learning | sklearn | Implement KNN, RF, SVM, and evaluation metrics |
| Deep Learning | tensorflow, keras, pytorch | CNN, CNN+Attention, ResNet models |
| Visualization | matplotlib, seaborn | Plot MRI images, distributions, and confusion matrices |

---

## 📂 Dataset Overview
- **Input Data:** MRI image files (`.jpg`, `.png`) containing axial, coronal, or sagittal slices.  
- **Target Labels:** Multi-class labels: `"Meningioma"`, `"Glioma"`, `"Pituitary Tumor"`, `"No Tumor"`.  
- **Preprocessing:** Segmentation pipelines used to extract regions of interest.

---

## 🚀 Getting Started
### Prerequisites
- Python 3.x  
- pip or conda package manager  

### Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
