# 🧠 Parkinson's Disease Detection Using Machine Learning

A machine learning-based system for early detection of Parkinson's disease 
using biomedical voice measurements. This project explores multiple 
classification algorithms to accurately identify Parkinson's disease from 
vocal features.

## 🎯 Project Overview

Parkinson's disease is a progressive neurological disorder affecting movement, 
speech, and motor control. Early diagnosis is critical but traditional methods 
rely heavily on clinical expertise, which can be subjective and time-consuming.

This project aims to automate the detection process using machine learning 
techniques applied to voice feature datasets, enabling faster and more 
reliable diagnoses.

## 📊 Dataset

- **Source:** UCI Machine Learning Repository (via Kaggle)
- **Samples:** 195 instances (147 Parkinson's, 48 Healthy)
- **Features:** 24 voice measurement attributes
- **Key features:** Jitter, Shimmer, Fundamental frequency, HNR, etc.

## 🔬 Methodology

### Data Preprocessing
- Column name standardization
- Missing value & duplicate checking
- Feature scaling with StandardScaler
- Correlation-based feature selection (dropped 11 highly correlated features)

### Machine Learning Models Implemented
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| **KNN** | **94.87%** | 94.12% | 100% | **96.97%** |
| SVM | 92.31% | 91.43% | 100% | 95.52% |
| Random Forest | 92.31% | 93.94% | 96.88% | 95.38% |
| Logistic Regression | 89.74% | 88.89% | 100% | 94.12% |
| AdaBoost | 89.74% | 91.18% | 96.88% | 93.94% |
| Decision Tree | 82.05% | 93.10% | 84.38% | 88.52% |

## 🏆 Key Results

**K-Nearest Neighbors (KNN)** achieved the best overall performance:
- Highest Accuracy: 94.87%
- Highest F1-Score: 96.97%
- Perfect Recall: 100%
- Best R²: 0.6518

## 🛠️ Technologies Used

- **Python 3**
- **Pandas** - Data manipulation
- **NumPy** - Numerical computing
- **Scikit-learn** - Machine learning models
- **Matplotlib & Seaborn** - Data visualization

## 📁 Repository Structure
├── Parkinson_Disease_Detection.ipynb
├── README.md 
└── data/
└── parkinsons.csv

Future Improvements
Test on larger, more diverse datasets

Implement deep learning approaches

Add multimodal data (handwriting, movement signals)

Deploy as a web application for clinical use

Implement SHAP for model interpretability

